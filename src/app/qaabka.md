  #  Make the HeroDetailComponent
  
```javascript
ng generate component hero-detailk
```

____

```javascript
<div *ngIf="hero">

  <h2>{{hero.name | uppercase}} Details</h2>
  <div><span>id: </span>{{hero.id}}</div>
  <div>
    <label for="hero-name">Hero name: </label>
    <input id="hero-name" [(ngModel)]="hero.name" placeholder="name">
  </div>

</div>
```
____

## Add the @Input() hero property
```javascript
import { Hero } from '../hero';
```
___
```javascript
import { Component, OnInit, Input } from '@angular/core';
```
___

```javascript

<app-hero-detail [hero]="selectedHero"></app-hero-detail>
```

