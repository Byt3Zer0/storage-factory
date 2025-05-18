# Byt3Zer0 Storage Factory

[![Build Status](https://img.shields.io/github/actions/workflow/status/Byt3Zer0/storage-factory/forge.yml?branch=main)](https://github.com/Byt3Zer0/storage-factory/actions)
[![License](https://img.shields.io/github/license/Byt3Zer0/storage-factory)](LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/Byt3Zer0/storage-factory)](https://github.com/Byt3Zer0/storage-factory/stargazers)

---

<p align="center">
  <img src="https://raw.githubusercontent.com/Byt3Zer0/storage-factory/main/thumbnails/storage-factory.png" alt="Storage Factory" width="300">
</p>

## 🏗️ Descripción

Este proyecto implementa el patrón **Factory** para desplegar múltiples instancias de `SimpleStorage` usando Foundry y Remix.

**Autor:** Byt3Zer0 ([GitHub](https://github.com/Byt3Zer0))

**Objetivo:** Crear un ejemplo práctico para mi portafolio de desarrollo blockchain.

## 📋 Índice

1. [Características](#-características)
2. [Estructura del proyecto](#-estructura-del-proyecto)
3. [Instalación](#-instalación)
4. [Uso](#-uso)
5. [Tests](#-tests)
6. [Comandos de Foundry](#-comandos-de-foundry)
7. [Contribuciones](#-contribuciones)
8. [Licencia](#-licencia)

## ✨ Características

- Despliega instancias de `SimpleStorage` de forma programática.
- Ejemplos de scripts para Foundry (`forge script`).
- Tests automatizados con Forge Standard Library.
- Integración opcional con Remix.

## 🗂️ Estructura del proyecto

```
├── src/
│   ├── SimpleStorage.sol
│   └── StorageFactory.sol
├── script/
│   └── DeployStorageFactory.s.sol
├── test/
│   └── StorageFactoryTest.t.sol
├── thumbnails/
│   └── storage-factory.png
├── README.md
└── LICENSE
```

## 🚀 Instalación

1. Clona tu fork:

   ```bash
   git clone https://github.com/Byt3Zer0/storage-factory.git
   cd storage-factory
   ```

2. Instala Foundry si no lo tienes:

   ```bash
   curl -L https://foundry.paradigm.xyz | bash
   source ~/.bashrc
   foundryup
   ```

3. Construye el proyecto:

   ```bash
   forge build
   ```

## ⚙️ Uso

- **Desplegar en local (Anvil):**

  ```bash
  anvil &
  forge script script/DeployStorageFactory.s.sol --broadcast --rpc-url http://127.0.0.1:8545
  ```

- **Interacción rápida en Remix:**

  1. Abre [Remix](https://remix.ethereum.org/).
  2. Copia los contratos de `src/`.
  3. Ejecuta el script de Factory desde la pestaña de Scripts.

## ✅ Tests

Ejecuta todos los tests con:

```bash
forge test -vv --gas-report
```

## 🔧 Comandos de Foundry

- `forge build`: compila los contratos.
- `forge test`: ejecuta los tests.
- `forge script`: ejecuta scripts de despliegue.

## 🤝 Contribuciones

¡Bienvenidas! Si encuentras errores o quieres mejorar el proyecto, abre un Issue o Pull Request.

## 📜 Licencia

Este proyecto está bajo la licencia MIT. Para más detalles, consulta el archivo [LICENSE](LICENSE).
