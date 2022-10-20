---
slug: /ITWMultichainRegistry
title: ITWMultichainRegistry
hide_title: true
displayed_sidebar: contracts
---

# ITWMultichainRegistry

## Methods

### add

```solidity
function add(address _deployer, address _deployment, uint256 _chainId, string metadataUri) external nonpayable
```

Add a deployment for a deployer.

#### Parameters

| Name         | Type    | Description |
| ------------ | ------- | ----------- |
| \_deployer   | address | undefined   |
| \_deployment | address | undefined   |
| \_chainId    | uint256 | undefined   |
| metadataUri  | string  | undefined   |

### count

```solidity
function count(address _deployer) external view returns (uint256 deploymentCount)
```

Get the total number of deployments for a deployer.

#### Parameters

| Name       | Type    | Description |
| ---------- | ------- | ----------- |
| \_deployer | address | undefined   |

#### Returns

| Name            | Type    | Description |
| --------------- | ------- | ----------- |
| deploymentCount | uint256 | undefined   |

### getAll

```solidity
function getAll(address _deployer) external view returns (struct ITWMultichainRegistry.Deployment[] allDeployments)
```

Get all deployments for a deployer.

#### Parameters

| Name       | Type    | Description |
| ---------- | ------- | ----------- |
| \_deployer | address | undefined   |

#### Returns

| Name           | Type                               | Description |
| -------------- | ---------------------------------- | ----------- |
| allDeployments | ITWMultichainRegistry.Deployment[] | undefined   |

### getMetadataUri

```solidity
function getMetadataUri(uint256 _chainId, address _deployment) external view returns (string metadataUri)
```

Returns the metadata IPFS URI for a deployment on a given chain if previously registered via add().

#### Parameters

| Name         | Type    | Description |
| ------------ | ------- | ----------- |
| \_chainId    | uint256 | undefined   |
| \_deployment | address | undefined   |

#### Returns

| Name        | Type   | Description |
| ----------- | ------ | ----------- |
| metadataUri | string | undefined   |

### remove

```solidity
function remove(address _deployer, address _deployment, uint256 _chainId) external nonpayable
```

Remove a deployment for a deployer.

#### Parameters

| Name         | Type    | Description |
| ------------ | ------- | ----------- |
| \_deployer   | address | undefined   |
| \_deployment | address | undefined   |
| \_chainId    | uint256 | undefined   |

## Events

### Added

```solidity
event Added(address indexed deployer, address indexed deployment, uint256 indexed chainId, string metadataUri)
```

#### Parameters

| Name                 | Type    | Description |
| -------------------- | ------- | ----------- |
| deployer `indexed`   | address | undefined   |
| deployment `indexed` | address | undefined   |
| chainId `indexed`    | uint256 | undefined   |
| metadataUri          | string  | undefined   |

### Deleted

```solidity
event Deleted(address indexed deployer, address indexed deployment, uint256 indexed chainId)
```

#### Parameters

| Name                 | Type    | Description |
| -------------------- | ------- | ----------- |
| deployer `indexed`   | address | undefined   |
| deployment `indexed` | address | undefined   |
| chainId `indexed`    | uint256 | undefined   |