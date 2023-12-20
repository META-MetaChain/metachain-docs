import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

import { MultiDimensionalContentWidget } from '@site/src/components/MultiDimensionalContentWidget.js';

<MultiDimensionalContentWidget />

<!-- todo: end the annoyance of this file not being clearly tightly coupled to the MultiDimensionalContentWidget.js file that lives somewhere else; probably move this file next to that other file -->

<div className='dynamic-content-tabs'>
  <Tabs className="tabgroup-with-label os-tabgroup" groupId="os" defaultValue="others" values={[
    {label: 'Operating system:', value: 'label'},
    {label: 'Linux, MacOS, Arm64', value: 'others'},
    {label: 'Windows', value: 'win'}
  ]}>
    <TabItem className="unclickable-element" value="label"></TabItem>
    <TabItem value="others"></TabItem>
    <TabItem value="win"></TabItem>
  </Tabs>

<Tabs
  className="tabgroup-with-label network-tabgroup"
  groupId="network"
  defaultValue="META-one-nitro"
  values={[
    { label: 'Network:', value: 'label' },
    { label: 'metachain One (Nitro)', value: 'META-one-nitro' },
    { label: 'metachain One (Classic)', value: 'META-one-classic' },
    { label: 'metachain Nova', value: 'META-nova' },
    { label: 'metachain Goerli', value: 'META-goerli' },
    { label: 'metachain Sepolia', value: 'META-sepolia' },
    { label: 'Localhost', value: 'localhost' },
  ]}
>
  <TabItem className="unclickable-element" value="label"></TabItem>
  <TabItem value="META-one-nitro"></TabItem>
  <TabItem value="META-one-classic"></TabItem>
  <TabItem value="META-nova"></TabItem>
  <TabItem value="META-goerli"></TabItem>
  <TabItem value="META-sepolia"></TabItem>
  <TabItem value="localhost"></TabItem>
</Tabs>

  <Tabs className="tabgroup-with-label node-type-tabgroup" groupId="node-type" defaultValue="full-node" values={[
        {label: 'Node type:', value: 'label'},
        {label: 'Full node', value: 'full-node'},
        {label: 'Archive node', value: 'archive-node'},
        {label: 'Validator node', value: 'validator-node'}
    ]}>
    <TabItem className="unclickable-element" value="label"></TabItem>
    <TabItem value="full-node"></TabItem>
    <TabItem value="archive-node"></TabItem>
    <TabItem value="validator-node"></TabItem>
  </Tabs>
</div>
