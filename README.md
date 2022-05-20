## Basics

- Interpolation `{{}}` for render some properties on the page;
- Property binding `[]` for setting values for properties of html-tags;
- Event binding `<button (click)="function()">My Button</button>` listens to events and responds with defined function;
- `*ngFor` & `*ngIf`

## Receive data from parent component

- Child imports `Input` from `@angular/core`;
- Also child: `@Input() object!: Class;`
- In parent HTML make `<childTag [property]="data"></childTag>` <br/>
  E.g. : `<app-product-alerts [product]="product"</app-product-alerts>`
  
## Pass data to parent component

- Child imports `Output` and `EventEmitter` from `@angular/core`;
- Also child: `@Output() notify = new EventEmmiter();`
- Child: `(click) = "notify.emit()"`;
- Parent shall contain function for response;
- Parent: `<child (notify)="function()">`;





## Hints

![image](https://user-images.githubusercontent.com/86207944/169402485-ad242223-36d2-4921-b0cc-808970938108.png)


