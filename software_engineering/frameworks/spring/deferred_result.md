# Deferred Result

## Basic idea

A Spring MVC return type that lets a controller return a placeholder *now* and resolve it from another thread *later*, freeing the servlet container thread during the wait. Useful for long-running or asynchronous work without holding a request thread.

## Key facts

- `DeferredResult<T>` releases the request thread until `setResult` / `setErrorResult` is called.
- Configurable timeout; lifecycle callbacks (`onCompletion`, `onTimeout`, `onError`).
- Alternatives: `Callable<T>`, `CompletableFuture<T>`, reactive `Mono`/`Flux` (WebFlux).

