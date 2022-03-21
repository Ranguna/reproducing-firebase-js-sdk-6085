# How to reproduce:

1. `npm i`
2. `npm run build`

The following compilations errors should popup:

```
> reproducing_firebase-js-sdk_6085@1.0.0 build
> tsc

node_modules/@firebase/util/dist/src/indexeddb.d.ts:19:23 - error TS2304: Cannot find name 'DOMStringList'.

19     objectStoreNames: DOMStringList;
                         ~~~~~~~~~~~~~

node_modules/@firebase/util/dist/src/indexeddb.d.ts:20:22 - error TS2304: Cannot find name 'IDBDatabase'.

20     constructor(_db: IDBDatabase);
                        ~~~~~~~~~~~

node_modules/@firebase/util/dist/src/indexeddb.d.ts:21:55 - error TS2304: Cannot find name 'IDBTransactionMode'.

21     transaction(storeNames: string[] | string, mode?: IDBTransactionMode): TransactionWrapper;
                                                         ~~~~~~~~~~~~~~~~~~

node_modules/@firebase/util/dist/src/indexeddb.d.ts:22:52 - error TS2304: Cannot find name 'IDBObjectStoreParameters'.

22     createObjectStore(storeName: string, options?: IDBObjectStoreParameters): ObjectStoreWrapper;
                                                      ~~~~~~~~~~~~~~~~~~~~~~~~

node_modules/@firebase/util/dist/src/indexeddb.d.ts:28:31 - error TS2304: Cannot find name 'IDBTransaction'.

28     constructor(_transaction: IDBTransaction);
                                 ~~~~~~~~~~~~~~

node_modules/@firebase/util/dist/src/indexeddb.d.ts:33:25 - error TS2304: Cannot find name 'IDBObjectStore'.

33     constructor(_store: IDBObjectStore);
                           ~~~~~~~~~~~~~~

node_modules/@firebase/util/dist/src/indexeddb.d.ts:35:57 - error TS2304: Cannot find name 'IDBIndexParameters'.

35     createIndex(name: string, keypath: string, options: IDBIndexParameters): IndexWrapper;
                                                           ~~~~~~~~~~~~~~~~~~

node_modules/@firebase/util/dist/src/indexeddb.d.ts:43:25 - error TS2304: Cannot find name 'IDBIndex'.

43     constructor(_index: IDBIndex);
                           ~~~~~~~~


Found 8 errors in the same file, starting at: node_modules/@firebase/util/dist/src/indexeddb.d.ts:19
```
