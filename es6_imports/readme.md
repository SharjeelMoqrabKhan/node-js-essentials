# ES6 Modules

ES6 is provading a new to import any module. There only 1 deualt module in file and other nth number exports we can do.

for using ES6 Modules we neet to use .mjs extension and have to use "type": "module", in package.json.

### age.mjs
```
export default function ageInMonths(age){
    return age*12;
}

export function ageInDays(age){
    return age*356;
}
```

### index.js
```
import ageInMonths,{ageInDays} from "./es6_imports/age.mjs";

const ageInMonth=ageInMonths(20);
console.log("Age in months",ageInMonth);

const ageInDay=ageInDays(20);
console.log("Age in days",ageInDay);
```