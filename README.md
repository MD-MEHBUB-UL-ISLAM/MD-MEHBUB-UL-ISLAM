# MD Mehbub Ul Islam

## Angular Developer | Open Source Creator | Performance Optimization Specialist

<p align="center">
  <a href="https://linkedin.com/in/md-mehbub-ul-islam-17b852257" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <a href="https://github.com/MD-MEHBUB-UL-ISLAM" target="_blank">
    <img src="https://img.shields.io/badge/GitHub-Follow-181717?style=for-the-badge&logo=github&logoColor=white" />
  </a>
  <a href="mailto:mdmehbubulislam@gmail.com">
    <img src="https://img.shields.io/badge/Email-Reach%20Out-EA4335?style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
</p>

---

## 🎯 About Me

I'm a **frontend-focused Angular engineer** with a passion for building high-performance, production-grade applications and reusable component libraries. My expertise spans modern Angular architecture (signals, standalone components), responsive UI design, internationalization, and performance optimization. I've published **6 npm packages** with a focus on solving real-world developer challenges.

**Key Strengths:**
- 🏗️ **Architecture & Design Patterns** – Standalone components, signal-based state management, dependency injection optimization
- ⚡ **Performance** – Virtual scrolling (100k+ items @ 60 FPS), memory-efficient rendering, bundle size optimization
- 🌍 **Scalability** – Bilingual (EN/BN) applications, responsive design systems, reusable component libraries
- 🧪 **Code Quality** – TypeScript strict mode, RxJS reactive patterns, maintainable, production-ready code

---

## 📦 Open Source Impact

### Published npm Packages

| Package | Purpose | Key Features |
|---------|---------|--------------|
| **ngx-virtual-scroller** | High-performance list rendering | Render 100k+ items at 60 FPS with constant memory |
| **ngx-ai-assist** | AI-powered components | Chat, autocomplete, content generator with OpenAI streaming |
| **ngx-dynamic-form-builder** | JSON-driven form generation | 15+ field types, validation, conditional logic |
| **ngx-date-range-picker** | Bilingual date selection | English/Bengali UI, responsive design, language toggle |
| **ngx-video-recorder** | Media capture | Pause/resume, playback, device selection, glass-morphism UI |
| **ngx-attack-detector** | Security monitoring | Script injection detection |

📊 **Stats:** 6 published packages | Focus on developer experience and performance

---

## 🛠️ Technical Expertise

### Core Technologies
```
Angular 19+  •  TypeScript  •  RxJS  •  Signals  •  Standalone Components
Tailwind CSS  •  Responsive Design  •  Transloco i18n  •  HTML5/CSS3
```

### Specializations
- **Frontend Architecture:** Standalone components, custom pipes, service-based patterns
- **State Management:** Angular signals, computed properties, reactive patterns
- **Component Libraries:** Reusable, documented, npm-published packages
- **Internationalization:** Bilingual (English/Bengali) applications with dynamic language switching
- **Performance Tuning:** Virtual scrolling, lazy loading, bundle optimization
- **Responsive Design:** Mobile-first development, breakpoint strategies, adaptive layouts

### Tools & Ecosystem
![Angular](https://img.shields.io/badge/Angular-DD0031?style=flat-square&logo=angular&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![RxJS](https://img.shields.io/badge/RxJS-B7178C?style=flat-square&logo=reactivex&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)

---

## 💼 What You'll Get Working With Me

✅ **Clean, maintainable code** following SOLID principles and Angular best practices  
✅ **Performance-first mindset** – optimized rendering, lazy loading, bundle size awareness  
✅ **Reusable components** – well-documented, tested, and production-ready  
✅ **Responsive expertise** – pixel-perfect designs across all devices  
✅ **Bilingual support** – seamless English/Bengali internationalization  
✅ **Proactive problem solver** – finds bottlenecks and implements solutions  

---

## 📈 Achievements

- 🎁 **Published 6 npm packages** on public registries
- 💡 **Developed high-performance solutions** for rendering 100k+ items at 60 FPS
- 🌐 **Built bilingual applications** with seamless EN/BN language switching
- 🚀 **Optimized applications** through virtual scrolling, lazy loading, and reactive patterns
- 📚 **Created reusable libraries** solving real-world developer challenges

---

## 🎓 How I Work

- **Modern Angular First** – Latest features (signals, standalone components, control flow syntax)
- **Type Safety** – Strict TypeScript, zero implicit any
- **Responsive & Mobile-Ready** – Tailwind CSS, mobile-first approach
- **Scalable & Maintainable** – Clean architecture, DRY principles, documented code
- **Performance Conscious** – Lazy loading, virtual scrolling, bundle optimization
- **Collaborative** – Clear communication, code reviews, knowledge sharing

---

## 🚀 Currently Building

**ngx-data-grid** – Advanced data grid component with sorting, filtering, pagination, and virtual scrolling *(coming soon)*

---

## 📞 Let's Connect!

💼 **Open to opportunities** in Angular frontend development, component library creation, and performance optimization roles.

- **LinkedIn:** [md-mehbub-ul-islam-17b852257](https://linkedin.com/in/md-mehbub-ul-islam-17b852257)
- **GitHub:** [MD-MEHBUB-UL-ISLAM](https://github.com/MD-MEHBUB-UL-ISLAM)
- **Email:** [mdmehbubulislam@gmail.com](mailto:mdmehbubulislam@gmail.com)

---

<div align="center">

### 💻 Sample Code Snippet

```typescript
// Signal-based component with computed properties
@Component({
  selector: 'app-job-listing',
  standalone: true,
  template: `
    @for (job of filteredJobs(); track job.id) {
      <div class="job-card">
        {{ job.title }} - {{ formatSalary(job.salary) }}
      </div>
    }
  `
})
export class JobListingComponent {
  jobs = signal<Job[]>([]);
  searchTerm = signal('');
  
  filteredJobs = computed(() =>
    this.jobs().filter(j => 
      j.title.includes(this.searchTerm())
    )
  );
}
```

---

<p align="center">
  <i>"Code quality is not just about functionality—it's about creating maintainable solutions that scale with your team."</i>
</p>

⭐ **[View my repositories →](https://github.com/MD-MEHBUB-UL-ISLAM)**

</div>
