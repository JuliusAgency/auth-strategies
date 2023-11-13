## Auth-strategies

The auth-strategies package - is a component of the @jla/node [packages set](https://github.com/JuliusAgency/node-packages-set) for Nodejs applications.  

<p>
  <a href="https://www.npmjs.com/package/@jla/auth-strategies" target="_blank">
    <img alt="Version" src="https://img.shields.io/npm/v/@jla/auth-strategies.svg">
  </a>
  <a href="https://github.com/JuliusAgency/auth-strategies#readme" target="_blank">
    <img alt="Documentation" src="https://img.shields.io/badge/documentation-yes-brightgreen.svg" />
  </a>
  <a href="https://github.com/JuliusAgency/auth-strategies/graphs/commit-activity" target="_blank">
    <img alt="Maintenance" src="https://img.shields.io/badge/Maintained%3F-yes-green.svg" />
  </a>
  <a href="https://github.com/JuliusAgency/auth-strategies/blob/master/LICENSE" target="_blank">
    <img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-yellow.svg" />
  </a>
</p>

### Installation
```bash
  npm install --save @jla/auth-strategies
```

### Pre-conditions:
```
The package is dedicated to be used with the following @jla packages:
  - @jla/base-user-mongo or @jla/base-user-sql
  - @jla/auth-jwt or auth-session;  
```

### Usage  
```
  import { initStrategies, StrategyOptions } from '@jla/auth-strategies';
  import { BaseUser, dBApi } from '@jla/base-user-sql'; // @jla/base-user-mongo


  // setup 
  const baseUser = sqlRepository(BaseUser);
  const strategyOptions: StrategyOptions = {
    passport: passport,
    dBApi: dBApi(baseUser),
  };
  const strategy = initStrategies(strategyOptions);

```
