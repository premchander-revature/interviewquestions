1. How do you make a service availiable for a component?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>
  
```ts
 @Component({
  selector: 'hero-list',
  template: '...',
  providers: [HeroService]
})
class HeroListComponent {}
```

</blockquote>
</details>
  
---

2. How do you make a service availiable for all the components of a NgModule?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>
  
```ts
@NgModule({
  declarations: [HeroListComponent]
  providers: [HeroService]
})
class HeroListModule {}
```
</blockquote>
</details>
  
---

3. How do you make a service availiable for the entire application?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

```ts
@Injectable({
  providedIn: 'root'
})
class HeroService {}
```

</blockquote>
</details>
  
---

4. How do you inject a dependency in angular?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>
  
```ts
@Component({ … })
class HeroListComponent {
  constructor(private service: HeroService) {}
}
```

</blockquote>
</details>
  
---
