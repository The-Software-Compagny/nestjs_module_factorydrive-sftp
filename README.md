<p align="center">
  <a href="http://nestjs.com/" target="blank">
    <img src="https://nestjs.com/img/logo_text.svg" width="320" alt="Nest Logo" />
  </a>
</p>

<p align="center">
  SFTP driver for Factory drive module from NestJS framework
</p>

<p align="center">
  <a href="https://www.npmjs.com/org/The-Software-Compagny"><img src="https://img.shields.io/npm/v/@the-software-compagny/nestjs_module_factorydrive-sftp.svg" alt="NPM Version" /></a>
  <a href="https://www.npmjs.com/org/The-Software-Compagny"><img src="https://img.shields.io/npm/l/@the-software-compagny/nestjs_module_factorydrive-sftp.svg" alt="Package License" /></a>
  <a href="https://github.com/The-Software-Compagny/nestjs_module_rcon/actions/workflows/ci.yml"><img src="https://github.com/The-Software-Compagny/nestjs_module_factorydrive-sftp/actions/workflows/ci.yml/badge.svg" alt="Publish Package to npmjs" /></a>
</p>
<br>

# SFTP driver for Factory drive module
SFTP driver for Factory drive module from NestJS framework

## Install dependencies
```bash
yarn add @the-software-compagny/nestjs_module_factorydrive @the-software-compagny/nestjs_module_factorydrive-sftp
```

## Usage
```ts
@Module({
  //...
})
export class AppModule {
  public constructor(storage: FactorydriveService) {
    // If you want to add a new driver you can use the registerDriver method
    storage.registerDriver('sftp', SFTPStorage)
  }
}
```
