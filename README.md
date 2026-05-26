# ⚡ ANGULAR COMPLETE MASTER GUIDE  
## 🚀 Beginner → Advanced → Pro Frontend Framework

---

# 📖 What is Angular?

### English
Angular is a powerful TypeScript-based frontend framework developed by Google for building dynamic single-page applications (SPA).

### বাংলা
Angular হলো Google-এর তৈরি TypeScript based frontend framework, যা দিয়ে SPA (Single Page Application) এবং large-scale web app বানানো যায়।

---

# 🌟 Why Angular?

- ⚡ Fast SPA Development
- 🧠 TypeScript Based
- 🏗️ Component Architecture
- 🔐 Built-in Security
- 🌐 REST API Support
- 📦 Scalable Enterprise Apps

---

# 🛠️ INSTALLATION

## Install Angular CLI

```bash
npm install -g @angular/cli
```

---

## Check Version

```bash
ng version
```

---

## Create Project

```bash
ng new my-app
```

---

## Run Project

```bash
cd my-app
ng serve
```

👉 Open:
```
http://localhost:4200
```

---

# 📁 PROJECT STRUCTURE

```
src/
 ├── app/
 │    ├── components/
 │    ├── services/
 │    ├── modules/
 │    ├── app.component.ts
 │    ├── app.module.ts
 ├── assets/
 ├── environments/
```

---

# ⚙️ BASIC COMMANDS

## Generate Component

```bash
ng generate component home
```

OR

```bash
ng g c home
```

---

## Generate Service

```bash
ng g service api
```

---

## Generate Module

```bash
ng g module auth
```

---

# 👋 BASIC COMPONENT

## app.component.ts

```ts
import { Component } from '@angular/core';

@Component({
  selector: 'app-root',
  templateUrl: './app.component.html'
})
export class AppComponent {
  title = 'Hello Angular';
}
```

---

## app.component.html

```html
<h1>{{ title }}</h1>
```

---

# 🔁 DATA BINDING

## Interpolation

```html
{{ name }}
```

---

## Property Binding

```html
<img [src]="imageUrl">
```

---

## Event Binding

```html
<button (click)="clickMe()">Click</button>
```

---

## Two Way Binding

```html
<input [(ngModel)]="name">
```

---

# 📦 DIRECTIVES

## ngIf

```html
<p *ngIf="isActive">Active</p>
```

---

## ngFor

```html
<li *ngFor="let item of items">{{item}}</li>
```

---

# 🧠 SERVICES

## Create Service

```bash
ng g service api
```

---

## Example Service

```ts
import { Injectable } from '@angular/core';

@Injectable({
  providedIn: 'root'
})
export class ApiService {

  getData(){
    return ["A", "B", "C"];
  }
}
```

---

# 🌐 HTTP / API CALL

## Import HttpClient

```ts
import { HttpClient } from '@angular/common/http';
```

---

## API Call Example

```ts
constructor(private http: HttpClient){}

getUsers(){
  return this.http.get("https://api.example.com/users");
}
```

---

# 🔐 ROUTING

## Setup Routes

```ts
import { RouterModule, Routes } from '@angular/router';

const routes: Routes = [
  { path: '', component: HomeComponent },
  { path: 'about', component: AboutComponent }
];
```

---

## Router Outlet

```html
<router-outlet></router-outlet>
```

---

# 🧱 COMPONENT COMMUNICATION

## Parent to Child

```ts
@Input() data: string;
```

---

## Child to Parent

```ts
@Output() event = new EventEmitter<string>();
```

---

# 📦 FORMS

## Template Driven Form

```html
<input [(ngModel)]="name">
```

---

## Reactive Form

```ts
form = new FormGroup({
  name: new FormControl('')
});
```

---

# ⚡ ANGULAR COMMANDS

```bash
ng new app-name
ng serve
ng build
ng generate component name
ng generate service name
ng generate module name
```

---

# 🗄️ API + BACKEND FLOW

```
Angular UI
    ↓
Service (HttpClient)
    ↓
REST API (Node/Django/Laravel)
    ↓
Database
    ↓
Response
```

---

# 🚀 BUILD PROJECT

```bash
ng build
```

Production Build:

```bash
ng build --configuration production
```

---

# 🧰 BEST TOOLS

## 💻 IDE
- VS Code (Best)
- WebStorm

---

## 🔌 EXTENSIONS
- Angular Language Service
- Prettier
- ESLint
- Angular Snippets

---

## 🌐 TOOLS
- Postman (API Testing)
- Chrome DevTools
- Git & GitHub

---

# 🏗️ PROJECT IDEAS

- Admin Dashboard
- E-commerce Frontend
- CRM System
- Blog Platform
- SaaS UI
- Inventory System
- ERP Dashboard

---

# 🏆 LEARNING ROADMAP

## 🟢 Beginner
- Components
- Templates
- Binding

## 🟡 Intermediate
- Services
- Routing
- Forms

## 🟠 Advanced
- API Integration
- Authentication
- Guards

## 🔴 Expert
- Large Scale Apps
- Performance Optimization
- Micro Frontend Architecture

---

# 💡 PRO TIPS

- Always use services for API
- Use modular architecture
- Lazy loading modules
- Optimize bundle size
- Use RxJS properly

---

# 👨‍💻 DEVELOPER

**Md. Moklasur Rahman Rahat**

🚀 Full Stack Developer  
⚡ Angular & Frontend Specialist  
💻 SaaS & Dashboard Builder  

GitHub: codexvisual

---

⭐ If you like this Angular guide, give it a star on GitHub
