---
title: "ion-breadcrumbs"
---
import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

import Props from '@site/static/auto-generated/breadcrumbs/props.md';
import Events from '@site/static/auto-generated/breadcrumbs/events.md';
import Methods from '@site/static/auto-generated/breadcrumbs/methods.md';
import Parts from '@site/static/auto-generated/breadcrumbs/parts.md';
import CustomProps from '@site/static/auto-generated/breadcrumbs/custom-props.md';
import Slots from '@site/static/auto-generated/breadcrumbs/slots.md';



import EncapsulationPill from '@components/page/api/EncapsulationPill';
import APITOCInline from '@components/page/api/APITOCInline';

<EncapsulationPill type="shadow" />

Breadcrumbs are navigation items that are used to indicate where a user is on an app or site. They should be used for large sites and apps with hierarchically arranged pages. Breadcrumbs can be collapsed based on the maximum number that can show, and the collapsed indicator can be clicked on to present a popover with more information or expand the collapsed breadcrumbs.

## Basic Usage

import Basic from '@site/static/usage/breadcrumbs/basic/index.md';

<Basic />

## Using Icons

### Icons on Items

import IconsOnItems from '@site/static/usage/breadcrumbs/icons/icons-on-items/index.md';

<IconsOnItems />

### Custom Separators

import CustomSeparators from '@site/static/usage/breadcrumbs/icons/custom-separators/index.md';

<CustomSeparators />

## Collapsing Items

### Max Items

If there are more items than the value of `maxItems`, the breadcrumbs will be collapsed. By default, only the first and last items will be shown.

import MaxItems from '@site/static/usage/breadcrumbs/collapsing-items/max-items/index.md';

<MaxItems />

### Items Before or After Collapse

Once the items are collapsed, the number of items to show can be controlled by the `itemsBeforeCollapse` and `itemsAfterCollapse` properties.

import ItemsBeforeAfter from '@site/static/usage/breadcrumbs/collapsing-items/items-before-after/index.md';

<ItemsBeforeAfter />

### Collapsed Indicator Click -- Expand Breadcrumbs

Clicking the collapsed indicator will fire the `ionCollapsedClick` event. This can be used to, for example, expand the breadcrumbs.

import ExpandOnClick from '@site/static/usage/breadcrumbs/collapsing-items/expand-on-click/index.md';

<ExpandOnClick />

### Collapsed Indicator Click -- Present Popover

The `ionCollapsedClick` event can also be used to present an overlay (in this case, an `ion-popover`) showing the hidden breadcrumbs.

import PopoverOnClick from '@site/static/usage/breadcrumbs/collapsing-items/popover-on-click/index.md';

<PopoverOnClick />

## Styling

## Color Property

import ColorProp from '@site/static/usage/breadcrumbs/styling/color/index.md';

<ColorProp />

## CSS Properties

import CSSProps from '@site/static/usage/breadcrumbs/styling/css-props/index.md';

<CSSProps />


## Properties
<Props />

## Events
<Events />

## Methods
<Methods />

## CSS Shadow Parts
<Parts />

## CSS Custom Properties
<CustomProps />

## Slots
<Slots />