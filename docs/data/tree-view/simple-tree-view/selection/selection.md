---
productId: x-tree-view
title: Simple Tree View - Selection
components: SimpleTreeView, TreeItem
packageName: '@mui/x-tree-view'
githubLabel: 'component: tree view'
waiAria: https://www.w3.org/WAI/ARIA/apg/patterns/treeview/
---

# Simple Tree View - Selection

<p class="description">Handle how users can select items.</p>

## Multi selection

The Tree View also supports multi-selection:

{{"demo": "MultiSelectTreeView.js"}}

## Disable selection

Use the `disableSelection` prop if you don't want your items to be selectable:

{{"demo": "DisableSelection.js"}}

## Controlled selection

Use the `selectedNodes` prop to control the selected items.

You can use the `onSelectedNodesChange` prop to listen to changes in the selected items and update the prop accordingly.

{{"demo": "ControlledSelection.js"}}

:::info

- The selection is **controlled** when its parent manages it by providing a `selectedNodes` prop.
- The selection is **uncontrolled** when it is managed by the component's own internal state. This state can be initialized using the `defaultSelectedNodes` prop.

Learn more about the _Controlled and uncontrolled_ pattern in the [React documentation](https://react.dev/learn/sharing-state-between-components#controlled-and-uncontrolled-components).
:::

## Track node selection change

Use the `onNodeSelectionToggle` prop if you want to react to a node selection change:

{{"demo": "TrackNodeSelectionToggle.js"}}
