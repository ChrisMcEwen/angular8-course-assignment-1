# Angular 8 Course - Assignment 1 Solution
My solution to Assignment 1 from https://www.udemy.com/the-complete-guide-to-angular-2/

I made the components without using ```ng generate component NewComponent``` / ```ng g c NewComponent```

### Steps
- Created new folders for the **SuccessAlert** and **WarningAlert** components and added .TS files for each
- Inside those .TS files I wrote:
- ```export class ClassName {}``` at the bottom
- ```import { Component } from '@angular/core';``` at the top
- ```@Component ({ selector: 'ElementSelector', template: `<div>stuff</div>` })``` as the meat in the sandwich (for styling, I used Bootstrap3 alert styles ```alert success-alert``` and ```alert danger-alert``` on the divs to get green and red stylish alerts
- Added these two lines to **app.module.ts**
```
import { SuccessAlert } from './SuccessAlert/success-alert-component';
import { WarningAlert } from './WarningAlert/warning-alert-component';
```
- Added **SuccessAlert** and **WarningAlert** to the ```declarations: ``` in **app.module.ts**
- Added the new components to **app.component.html** using the ```<SuccessAlert></SuccessAlert>``` and ```<WarningAlert</WarningAlert>``` element selectors

