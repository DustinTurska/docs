---
slug: /react.usemarketplace
title: useMarketplace() function
hide_title: true
displayed_sidebar: react
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

## useMarketplace() function

Hook for getting an instance of a `Marketplace` contract. This contract is used to support marketplace for purchase and sale of on-chain assets.

## Example

```javascript
import { useMarketplace } from '@thirdweb-dev/react'

export default function Component() {
  const marketplace = useMarketplace("<YOUR-CONTRACT-ADDRESS>")

  // Now you can use the marketplace contract in the rest of the component

  // For example, this function will return all the listings on the marketplace
  async function getListings() {
    const listings = await marketplace.getAll()
    return listings
  }

  ...
}
```

**Signature:**

```typescript
export declare function useMarketplace(
  contractAddress?: string,
): Marketplace | undefined;
```

## Parameters

| Parameter       | Type   | Description                                                                                 |
| --------------- | ------ | ------------------------------------------------------------------------------------------- |
| contractAddress | string | <i>(Optional)</i> the address of the Marketplace contract, found in your thirdweb dashboard |

**Returns:**

Marketplace \| undefined