---
title: Introduction
weight: 1

dashboardWeight: 0.2
dashboardState: incomplete
dashboardAudit: 0
---

# Introduction
---

Filecoin is a distributed storage network based on a blockchain mechanism.
Filecoin *miners* can elect to provide storage capacity for the network, and thereby
earn units of the Filecoin cryptocurrency (FIL) by periodically producing
cryptographic proofs that certify that they are providing the capacity specified.
In addition, Filecoin enables parties to exchange FIL currency
through transactions recorded in a shared ledger on the Filecoin blockchain.
Rather than using Nakamoto-style proof of work to maintain consensus on the chain, however,
Filecoin uses proof of storage itself: a miner's power in the consensus protocol
is proportional to the amount of storage it provides.

The Filecoin blockchain not only maintains the ledger for FIL transactions and
accounts, but also implements the Filecoin VM, a replicated state machine which executes
a variety of cryptographic contracts and market mechanisms among participants
on the network.
These contracts include *storage deals*, in which clients pay FIL currency to miners
in exchange for storing the specific file data that the clients request.
Via the distributed implementation of the Filecoin VM, storage deals
and other contract mechanisms recorded on the chain continue to be processed
over time, without requiring further interaction from the original parties
(such as the clients who requested the data storage).

## Spec Status

Each section of the spec must be stable and audited before it is considered done. The state of each section is tracked below. 

- The **State** column indicates the stability as defined in the legend. 
- The **Theory Audit** column shows the date of the last theory audit with a link to the report.
- The **Weight** column is used to highlight the relative criticality of a section against the others.

### Spec Status Legend

<table class="Dashboard">
  <thead>
    <tr>
      <th>Spec state</th>
      <th>Label</th>
    <tr>
  <thead>
  <tbody>
    <tr>
      <td>Final, will not change before mainnet launch</td>
      <td class="text-black bg-stable">Stable</td>
    </tr>
    <tr>
      <td>Correct, but some details are missing</td>
      <td class="text-black bg-incomplete">Incomplete</td>
    </tr>
    <tr>
      <td>Likely to change. Details still being finalised</td>
      <td class="text-black bg-wip">WIP</td>
    </tr>
    <tr>
      <td>Do not follow. Important things have changed</td>
      <td class="text-black bg-incorrect">Incorrect</td>
    </tr>
  </tbody>
</table>

### Spec Status Overview
<div id="test-dash"></div>

### Spec Stabilization Progess

This progress bar shows what percentage of the spec sections are considered stable.

{{<dashboard-progress>}}


### Implementations Status

Known implementations of the filecoin spec are tracked below, with their current CI build status, their test coverage as reported by [codecov.io](https://codecov.io), and a link to their last security audit report where one exists.

{{<dashboard-impl>}}