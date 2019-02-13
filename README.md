### chalk
---
https://github.com/chalk/chalk

```js
const chalk = require('chalk');
console.log(chalk.blue('Hello'));

const chalk = require('chalk');
const log = console.log;

log(chalk.blue('Hello') + ' World' + chalk.red('!'));
log(chalk.blue.bgRed.bold('Hello'));
log(chalk.blue('Hello', 'World!', 'Foo', 'bar', 'biz', 'baz'));
log(chalk.red('Hello', chalk.underline.bgBlue('world') + '!'));
log(chalk.green(
  'I am a green line ' +
  chalk.blue.underline.bold('with a blue substring') + 
  ' that becomes green again!'
));
log(`
CPU: ${chalk.red('90%')}
RAM: ${chalk.green('40%')}
DISK: ${chalk.yellow('70%')}
`);

log(chalk`
CPU: {red ${cpu.totalPercent}%}
RAM: {green ${ram.used /ram.total * 100}%}
DISK: {rgb(255,131,0) ${disk.used /disk.total * 100}%}
`);
log(chalk.keyword('orange')('Yay for orange colored text!'));
log(chalk.rgb(123, 45, 67).underline('Underlined reddish color'));
log(chalk.hex('#DEADED').bold('Bold gray!'));

const chalk = require('chalk');
const error = chalk.bold.red;
const waring = chalk.keyword('orange');
console.log(error('Error!'));
console.log(warning('Warning!'));

const name = 'Sindre';
console.log(chalk.green('Hello %s'), name);

const ctx = new chalk.constructor({enabled: false});
const ctx = new chalk.constructor({level: 0});

const chalk = require('chalk');
const miles = 18;
const calculateFeet = miles => miles * 5280;
console.log(chalk`
  There are {} in a mile.
  In {bold ${miles} miles}, there are {green.bold ${calculateFeet(miles)} feet}.
`);

console.log(chalk.bold.rgb(10, 100, 200)('Hello'));
console.log(chalk`{bold.rgb(10,100,200) Hello}`);
```

```
```

