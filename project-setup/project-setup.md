# Project setup

The **npm** is the primary way to install the **sigmajs**, create projects, and manage your Unity experience. It provides a central location to manage your Editor installations, Accounts and Licenses, and Projects.



```typescript
session
  .instruments()
  .pipe(
    map(it =>
      it.filter(x => x.quote.toString() == assetOf('binance:btc').toString())
    ),
    switchMap(it => zip(it.map(x => session.orderbook(x).pipe(take(1))))),
    tap(it => console.log(it.length))
  )
  .subscribe();
```



```
First of all you net to make sure that npm is installed
```



