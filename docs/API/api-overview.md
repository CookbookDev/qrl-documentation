---
docstatus: DRAFT
id: qrl-api-overview
title: QRL API Overview
hide_title: false
hide_table_of_contents: false
sidebar_label: API Overview
sidebar_position: 1
pagination_label: API Overview
custom_edit_url: https://github.com/theqrl/documentation/edit/master/docs/basics/what-is-qrl.md
description: QRL API Overview
keywords:
  - docs
  - build
  - developers
  - API
  - Overview
image: /assets/img/icons/yellow.png
slug: /api/qrl-api-overview
---



:::caution DOCUMENT STATUS 

<span>This document is in: <b>{frontMatter.docstatus}</b> status and needs additional input!</span>
:::



import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';
import CodeBlock from '@theme/CodeBlock';


The QRL API's are the portal into the inner workings of the Quantum Resistant Ledger's blockchain and wallet functions.

These API allow developers and advanced users access to core functions and information from the blockchain.

:::info
While there is no authentication required to interact with most of the QRL's API's, you will need to be able to reach the API service IP and Port of the node you are attempting to connect to. 

Best practice is to [run your own QRL node](/use/node/overview).
:::

## gRPC

The QRL API is organized around [gRPC (Google Remote Procedure Call)](https://grpc.io/). GRPC uses [protocol buffers](https://developers.google.com/protocol-buffers/docs/overview) for serializing structured data. 

Every function requires an object as parameter and returns another object as response. Our qrl.proto file lists the different objects as messages in two categories, request (named \*Req) and response (named \*Resp).

:::info
More information on GRPC can be found in [their official documentation](https://grpc.io/)
:::

<Tabs defaultValue="public" 
      groupID="syntaxSelection" 
      values={[
        { label: 'Public API', value: 'public', },
        { label: 'Wallet API', value: 'wallet', },
        { label: 'Walletd-Rest API', value: 'walletd-rest', },
        { label: 'Zeus Proxy', value: 'zeus-proxy', },
        { label: 'Explorer API', value: 'explorer', },
      ]}>
  
  <TabItem value="public">
    <h2>QRL Public API</h2>
    <p>The core QRL API responsible for all blockchain functions.</p>
    <span>
      <section class="row list_node_modules-@docusaurus-theme-classic-lib-theme-DocCategoryGeneratedIndexPage-styles-module">
        <article class="col col--6 margin-bottom--lg">
          <a class="card padding--lg cardContainer_node_modules-@docusaurus-theme-classic-lib-theme-DocCard-styles-module" href="/api/qrl-public-api">
            <h2 class="text--truncate cardTitle_node_modules-@docusaurus-theme-classic-lib-theme-DocCard-styles-module" title="QRL Wallet">
              QRL Public API
            </h2>
            <p class="text--truncate cardDescription_node_modules-@docusaurus-theme-classic-lib-theme-DocCard-styles-module" title="Creating Addresses, Sending and Receiving QRL">Core blockchain functions and operations.</p>
          </a>
        </article>
      </section>
    </span>
  </TabItem>
  
  <TabItem value="wallet">
    <h2>QRL Wallet API</h2>
    <p>The core wallet API functions.</p>
    <span>
      <section class="row list_node_modules-@docusaurus-theme-classic-lib-theme-DocCategoryGeneratedIndexPage-styles-module">
        <article class="col col--12 margin-bottom--lg">
          <a class="card padding--lg cardContainer_node_modules-@docusaurus-theme-classic-lib-theme-DocCard-styles-module" href="/api/wallet-api">
            <h2 class="text--truncate cardTitle_node_modules-@docusaurus-theme-classic-lib-theme-DocCard-styles-module" 
                title="What Is The QL">
              QRL Wallet API       
            </h2>
            <p class="text--truncate cardDescription_node_modules-@docusaurus-theme-classic-lib-theme-DocCard-styles-module" 
               title="Project explainer and information.">The QRL Wallet API documentation.</p>
          </a>
        </article>
      </section>
    </span>
  </TabItem>
  <TabItem value="walletd-rest">
    <h2>Walletd Rest Proxy - API</h2>
    <p>...</p>
    <span>
      <section class="row list_node_modules-@docusaurus-theme-classic-lib-theme-DocCategoryGeneratedIndexPage-styles-module">
        <article class="col col--12 margin-bottom--lg">
          <a class="card padding--lg cardContainer_node_modules-@docusaurus-theme-classic-lib-theme-DocCard-styles-module" href="/api/walletd-rest-proxy">
            <h2 class="text--truncate cardTitle_node_modules-@docusaurus-theme-classic-lib-theme-DocCard-styles-module" 
                title="Developers Overview">
              QRL Walletd Rest Proxy API      
            </h2>
            <p class="text--truncate cardDescription_node_modules-@docusaurus-theme-classic-lib-theme-DocCard-styles-module" 
               title="Developers general information.">Developers general information.</p>
          </a>
        </article>
      </section>
    </span>
  </TabItem>
  <TabItem value="zeus-proxy">
    <h2>Zeus Proxy API</h2>
    <p>...</p>
    <span>
      <section class="row list_node_modules-@docusaurus-theme-classic-lib-theme-DocCategoryGeneratedIndexPage-styles-module">
        <article class="col col--12 margin-bottom--lg">
          <a class="card padding--lg cardContainer_node_modules-@docusaurus-theme-classic-lib-theme-DocCard-styles-module" href="/api/zeus-proxy">
            <h2 class="text--truncate cardTitle_node_modules-@docusaurus-theme-classic-lib-theme-DocCard-styles-module" 
                title="Node Tutorials">
              Zeus Proxy API
            </h2>
            <p class="text--truncate cardDescription_node_modules-@docusaurus-theme-classic-lib-theme-DocCard-styles-module" 
               title="QRL Node related tutorials.">QRL Zeus Proxy API Documentation.</p>
          </a>
        </article>
      </section>
    </span>
  </TabItem>

  <TabItem value="explorer">
    <h2>Explorer API</h2>
    <p>...</p>
    <span>
      <section class="row list_node_modules-@docusaurus-theme-classic-lib-theme-DocCategoryGeneratedIndexPage-styles-module">
        <article class="col col--12 margin-bottom--lg">
          <a class="card padding--lg cardContainer_node_modules-@docusaurus-theme-classic-lib-theme-DocCard-styles-module" href="/api/explorer-api">
            <h2 class="text--truncate cardTitle_node_modules-@docusaurus-theme-classic-lib-theme-DocCard-styles-module" 
                title="Node Tutorials">
              QRL Explorer API
            </h2>
            <p class="text--truncate cardDescription_node_modules-@docusaurus-theme-classic-lib-theme-DocCard-styles-module" 
               title="QRL Node related tutorials.">QRL Explorer API documentation.</p>
          </a>
        </article>
      </section>
    </span>
  </TabItem>  
</Tabs>