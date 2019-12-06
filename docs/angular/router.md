# Router

## Grundlagen

### Routingstrategien

### Routen ausgeben

```typescript
import {Component, OnInit } from '@angular/core';
import { Router } from '@angular/router';


@Component(...)
class ExampleComponent implements OnInit {

  constructor (private router: Router) {
  }

   ngOnInit() {
     console.log('Configured routes: ', this.router.config);
   }
}
```

