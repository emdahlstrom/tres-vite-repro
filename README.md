# Vite Tres Skybox reproduction

Tested with bun and pnpm.

Adding the Sky abstraction and running bun dev results in:

```
Uncaught (in promise) TypeError: _ is undefined
    v tres.js:1062
    i tres.js:1062
    mountElement runtime-core.esm-bundler.js:5524
    processElement runtime-core.esm-bundler.js:5471
    patch runtime-core.esm-bundler.js:5339
    componentUpdateFn runtime-core.esm-bundler.js:6027
    run reactivity.esm-bundler.js:177
    update runtime-core.esm-bundler.js:6151
    setupRenderEffect runtime-core.esm-bundler.js:6161
    mountComponent runtime-core.esm-bundler.js:5929
    processComponent runtime-core.esm-bundler.js:5883
    patch runtime-core.esm-bundler.js:5351
    patchKeyedChildren runtime-core.esm-bundler.js:6346
    patchChildren runtime-core.esm-bundler.js:6218
    processFragment runtime-core.esm-bundler.js:5857
    patch runtime-core.esm-bundler.js:5325
    componentUpdateFn runtime-core.esm-bundler.js:6107
    run reactivity.esm-bundler.js:177
    update runtime-core.esm-bundler.js:6151
    callWithErrorHandling runtime-core.esm-bundler.js:195
    flushJobs runtime-core.esm-bundler.js:410
    promise callback*queueFlush runtime-core.esm-bundler.js:319
    queueJob runtime-core.esm-bundler.js:313
    effect runtime-core.esm-bundler.js:6145
    resetScheduling reactivity.esm-bundler.js:263
    trigger reactivity.esm-bundler.js:403
    updateSlots runtime-core.esm-bundler.js:4499
    updateComponentPreRender runtime-core.esm-bundler.js:6169
    componentUpdateFn runtime-core.esm-bundler.js:6084
    run reactivity.esm-bundler.js:177
    update runtime-core.esm-bundler.js:6151
    updateComponent runtime-core.esm-bundler.js:5960
    processComponent runtime-core.esm-bundler.js:5894
    patch runtime-core.esm-bundler.js:5351
    componentUpdateFn runtime-core.esm-bundler.js:6107
    run reactivity.esm-bundler.js:177
    update runtime-core.esm-bundler.js:6151
    rerender runtime-core.esm-bundler.js:493
    rerender runtime-core.esm-bundler.js:485
    tryWrap runtime-core.esm-bundler.js:551
    <anonymous> App.vue:56
    accept hmr.ts:77
    fetchUpdate hmr.ts:312
    queueUpdate hmr.ts:277
    queueUpdate hmr.ts:277
    handleMessage client.ts:205
    handleMessage client.ts:203
    setupWebSocket client.ts:91
    setupWebSocket client.ts:90
    <anonymous> client.ts:67
tres.js:1062:33

```
