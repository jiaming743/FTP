[ENGLISH](./README_EN.md)

<h1 align="center">FTP</h1>

<p align="center">
    <a href="https://github.com/jiaming743/ftp/blob/master/LICENSE">
      <img src="https://img.shields.io/github/license/jiaming743/ftp.svg" alt="LICENSE" />
    </a>
    <a href="https://www.npmjs.com/package/@jiaminghi/ftp">
      <img src="https://img.shields.io/npm/v/@jiaminghi/ftp.svg" alt="LICENSE" />
    </a>
</p>

### 基于 FTP 封装的 Promisify FTP

- **[put](#put)**

- **[rmDir](#rmDir)**

- **[mkDir](#mkDir)**

- **[getList](#getList)**

- **[emptyDir](#emptyDir)**

- **[deleteFile](#deleteFile)**

### npm 安装

```shell
$ npm install @jiaminghi/ftp
```

### 使用

```typescript
import { put, mkDir } from '@jiaminghi/ftp'

// do something
```

<h3 align="center">示例</h3>

#### put

```typescript
type put = (ftp: Client, src: string, dest: string) => Promise<boolean>
```

#### rmDir

```typescript
type rmDir = (ftp: Client, src: string, recusive = true) => Promise<boolean>
```

#### mkDir

```typescript
type mkDir = (ftp: Client, src: string, recusive = true) => Promise<boolean>
```

#### getList

```typescript
type getList = (ftp: Client, src: string) => Promise<Client.ListingElement[] | false>
```

#### emptyDir

```typescript
type emptyDir = (ftp: Client, src: string, except: string[] = []) => Promise<boolean>
```

#### deleteFile

```typescript
type deleteFile = (ftp: Client, src: string) => Promise<boolean>
```
