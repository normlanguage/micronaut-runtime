# micronaut.runtime Skill

Use this skill to work with Norm module `micronaut.runtime` version 4. Use only declarations listed below.

## `micronaut.runtime.context`

Source: `context/ApplicationContextLifeCycle.norm`

### `ApplicationContextLifeCycle`

```norm
interface ApplicationContextLifeCycle<T extends ApplicationContextLifeCycle<T>> extends ApplicationContextProvider, LifeCycle<T>
```

Type parameters:

- `T` extends `ApplicationContextLifeCycle<T>`

#### `close`

```norm
Void close()
```

Returns: `Void`

## `micronaut.runtime.context`

Source: `context/ApplicationContextProvider.norm`

### `ApplicationContextProvider`

```norm
interface ApplicationContextProvider
```

## `micronaut.runtime.context`

Source: `context/LifeCycle.norm`

### `LifeCycle`

```norm
interface LifeCycle<T extends LifeCycle<T>> extends Closeable, AutoCloseable
```

Type parameters:

- `T` extends `LifeCycle<T>`

#### `close`

```norm
Void close()
```

Returns: `Void`

## `micronaut.runtime.runtime`

Source: `runtime/EmbeddedApplication.norm`

### `EmbeddedApplication`

```norm
interface EmbeddedApplication<T extends EmbeddedApplication<T>> extends ApplicationContextLifeCycle<T>
```

Type parameters:

- `T` extends `EmbeddedApplication<T>`

#### `close`

```norm
Void close()
```

Returns: `Void`

## `micronaut.runtime.runtime.server`

Source: `runtime/server/EmbeddedServer.norm`

### `EmbeddedServer`

```norm
interface EmbeddedServer extends EmbeddedApplication<EmbeddedServer>
```

#### `close`

```norm
Void close()
```

Returns: `Void`

#### `getHost`

```norm
String? getHost()
```

Returns: `String?`

#### `getPort`

```norm
Integer getPort()
```

Returns: `Integer`

#### `getURI`

```norm
URI? getURI()
```

Returns: `URI?`

#### `isServer`

```norm
Boolean isServer()
```

Returns: `Boolean`

