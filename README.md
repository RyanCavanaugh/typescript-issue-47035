# typescript-issue-47035
Repro for https://github.com/microsoft/TypeScript/issues/47035

After checking out this repository invoke the following commands.

Build project_a
```
tsc -p project_a/tsconfig.json
```

Build project_b

```
tsc -p project_b/tsconfig.json
```

The following error is thrown
```
project_a/tsc/main.d.ts:2:36 - error TS2694: Namespace 'w' has no exported member 'IFuseOptions'.

2 export declare type Options = Fuse.IFuseOptions<string>;
                                     ~~~~~~~~~~~~


Found 1 error.
```
