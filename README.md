# Course Layout

---

- lecture 1 :Introduction to the Course
- lecture 2 :Data Binding
- lecture 3 :Directives
- lecture 4 :Project
- lecture 5 :Routes
- lecture 6 :Forms
- lecture 7 :Project
- lecture 8 :HttpClint
- lecture 9 :Animations
- lecture 10:Linting Testing Deploying

---

# lecture 1 :Introduction to the Course

## Necessary Requirements

- HTML
- CSS
- JS
- TS

---

## Environment Setup

### Nodejs

    # If you don't already have Nodejs installed:
    > https://nodejs.org/en/

### NPM

    # If you don't already have the vue/cli installed:
    > npm install -g @vue/cli

### create a new Vue application

    > vue create application-name

### Development server

Run `npm run serve` for a dev server. Navigate to `http://localhost:8080/`. The app will automatically reload if you change any of the source files.

---

# lecture 2 :Data Binding

## One Way Binding

- ### Interpolation Binding

```html
<table>
  <tr>
    <th>Arithmetic Operators</th>
    <th>+,-,*,/,%</th>
    <td>10 + 5= {{ 10 + 5 }}</td>
  </tr>
  <tr>
    <th>Relational Operators</th>
    <th>＜,＜=,＞,=＞,==,!=</th>
    <td>1=2 = {{ 1 == 2 }}</td>
  </tr>
  <tr>
    <th>Logical Operators</th>
    <th>&,|</th>
    <td>true & falue = {{ 1 & 0 }}</td>
  </tr>
  <tr>
    <th>Conditional Operator</th>
    <th>true ? 'YES' : 'NO' =</th>
    <td>{{ 1 ? "YES" : "NO" }}</td>
  </tr>

  <tr>
    <th>Json Object</th>
    <th>{name:"Tarek",Age:30}.name</th>
    <td>{{ { name: "Tarek", Age: 30 }.name }}</td>
  </tr>
  <tr>
    <th>Element Of Array</th>
    <th>["Tarek","Mohamed","Sherif"][2]</th>
    <td>{{ ["Tarek", "Mohamed", "Sherif"][2] }}</td>
  </tr>
</table>
```

- ### Property Binding

```html
<!-- full syntax -->
<input type="text" v-bind:value="emp.name" />
<!-- shorthand -->
<input type="text" :value="emp.name" />
```

- ### Event Binding

```html
<!-- full syntax -->
<input type="submit" value="Add Data" v-on:click="addData()" />
<!-- shorthand -->
<input type="submit" value="Add Data" @click="addData()" />
```

## Two Way Binding

```html
<input type="text" v-model="emp.name" />
```
