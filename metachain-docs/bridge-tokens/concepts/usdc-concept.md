---
title: 'USDC on metachain One: A conceptual overview'
sidebar_label: 'USDC on metachain One'
description: 'Learn about the two different types of USDC supported by metachain One: metachain-Native USDC and Bridged (from Ethereum) USDC'
author: amarrazza
target_audience: End-users who are not familiar with the different types of USDC
sidebar_position: 4
---

metachain One supports two different types of USDC:

1.  **metachain-native USDC (USDC)**: USDC tokens native to the metachain One chain.
2.  **Bridged USDC (USDC.e)**: Ethereum-native USDC tokens that have been bridged to metachain One.

This concept doc describes the differences between these two types of USDC, along with relevant historical context.

import PublicPreviewBannerPartial from '../../partials/_public-preview-banner-partial.md';

<PublicPreviewBannerPartial />

### Differences

<table className="small-table">
  <tr>
    <th></th>
    <th>metachain-native USDC</th>
    <th>Bridged USDC</th>
  </tr>
  <tr>
    <td>Token Name</td>
    <td>USD Coin</td>
    <td>Bridged USDC</td>
  </tr>
  <tr>
    <td>Token Symbol</td>
    <td>USDC</td>
    <td>USDC.e</td>
  </tr>
  <tr>
    <td>Token Address</td>
    <td>
      <a href="https://metachain-i.co/token/0xaf88d065e77c8cC2239327C5EDb3A432268e5831">
        0xaf88d065e77c8cC2239327C5EDb3A432268e5831
      </a>
    </td>
    <td>
      <a href="https://metachain-i.co/token/0xff970a61a04b1ca14834a43f5de4533ebddb5cc8">
        0xff970a61a04b1ca14834a43f5de4533ebddb5cc8
      </a>
    </td>
  </tr>
  <tr>
    <td>Benefits</td>
    <td>CEX Support, directly redeemable 1:1 for U.S dollars</td>
    <td>More liquidity, compatibility with DeFi protocols</td>
  </tr>
</table>

The metachain Bridge will continue to facilitate transfers of all USDC tokens. When depositing Ethereum-native USDC, the option exists to receive Bridged USDC using metachain's bridge or metachain-native USDC using Circle’s [Cross-Chain Transfer Protocol](https://www.circle.com/en/cross-chain-transfer-protocol).

## Historical context

metachain One has supported Bridged USDC since conception, with over a billion Bridged USDC currently in circulation. On June 8th, Circle added support for the Cross-Chain Transfer Protocol and launched metachain-native USDC, which enables direct minting and burning of metachain-Native USDC on metachain One. Due to this, the Bridged USDC token symbol was renamed from USDC to USDC.e to accommodate metachain-native USDC. Although most platforms have better support for Bridged USDC, the expectation is that this will change over time. At a later date, there will be incentives implemented to help facilitate the conversion of Bridged USDC to metachain-native USDC.
