## Description

`sp-tags` and `sp-tag` elements allow users to categorize content. They can represent keywords or people, and are grouped to describe an item or a search request.

### Usage

[![See it on NPM!](https://img.shields.io/npm/v/@spectrum-web-components/tags?style=for-the-badge)](https://www.npmjs.com/package/@spectrum-web-components/tags)
[![How big is this package in your project?](https://img.shields.io/bundlephobia/minzip/@spectrum-web-components/tags?style=for-the-badge)](https://bundlephobia.com/result?p=@spectrum-web-components/tags)
[![Try it on webcomponents.dev](https://img.shields.io/badge/Try%20it%20on-webcomponents.dev-green?style=for-the-badge)](https://webcomponents.dev/edit/collection/fO75441E1Q5ZlI0e9pgq/416WQzw187aA7udkjT8a/src/index.ts)

```
yarn add @spectrum-web-components/tags
```

Import the side effectful registration of `<sp-tags>` or `<sp-tag>` via:

```
import '@spectrum-web-components/tags/sp-tags.js';
import '@spectrum-web-components/tags/sp-tag.js';
```

When looking to leverage the `Tags` or `Tag` base classes as a type and/or for extension purposes, do so via:

```
import {
    Tags,
    Tag
} from '@spectrum-web-components/tags';
```

## Example

```html-live
<sp-tags>
    <sp-tag>Tag 1</sp-tag>
    <sp-tag invalid>Tag 2</sp-tag>
    <sp-tag disabled>Tag 3</sp-tag>
</sp-tags>
```

```html-live
<sp-tags>
    <sp-tag>
        Tag 1
        <sp-avatar
            slot="avatar"
            label="Tag 1"
            src=https://place.dog/500/500
        ></sp-avatar>
    </sp-tag>
    <sp-tag invalid>
        Tag 2
        <sp-avatar
            slot="avatar"
            label="Tag 1"
            src=https://place.dog/500/500
        ></sp-avatar>
    </sp-tag>
    <sp-tag disabled>
        Tag 3
        <sp-avatar
            slot="avatar"
            label="Tag 1"
            src=https://place.dog/500/500
        ></sp-avatar>
    </sp-tag>
</sp-tags>
```

```html-live
<sp-tags>
    <sp-tag>
        Tag 1
        <sp-icon-magnify slot="icon" size="s"></sp-icon-magnify>
    </sp-tag>
    <sp-tag invalid>
        Tag 2
        <sp-icon-magnify slot="icon" size="s"></sp-icon-magnify>
    </sp-tag>
    <sp-tag disabled>
        Tag 3
        <sp-icon-magnify slot="icon" size="s"></sp-icon-magnify>
    </sp-tag>
</sp-tags>
```

### Deletable

Use the `deletable` attribute to signify `sp-tags` elements that can be removed. The tags will only be focusable when they have the `deletable` attribute.

```html-live
<sp-tags>
    <sp-tag deletable>Tag 1</sp-tag>
    <sp-tag invalid deletable>Tag 2</sp-tag>
    <sp-tag disabled deletable>Tag 3</sp-tag>
</sp-tags>
```

```html-live
<sp-tags>
    <sp-tag deletable>
        Tag 1
        <sp-avatar
            slot="avatar"
            label="Tag 1"
            src=https://place.dog/500/500
        ></sp-avatar>
    </sp-tag>
    <sp-tag invalid deletable>
        Tag 2
        <sp-avatar
            slot="avatar"
            label="Tag 1"
            src=https://place.dog/500/500
        ></sp-avatar>
    </sp-tag>
    <sp-tag disabled deletable>
        Tag 3
        <sp-avatar
            slot="avatar"
            label="Tag 1"
            src=https://place.dog/500/500
        ></sp-avatar>
    </sp-tag>
</sp-tags>
```

```html-live
<sp-tags>
    <sp-tag deletable>
        Tag 1
        <sp-icon-magnify slot="icon" size="s"></sp-icon-magnify>
    </sp-tag>
    <sp-tag invalid deletable>
        Tag 2
        <sp-icon-magnify slot="icon" size="s"></sp-icon-magnify>
    </sp-tag>
    <sp-tag disabled deletable>
        Tag 3
        <sp-icon-magnify slot="icon" size="s"></sp-icon-magnify>
    </sp-tag>
</sp-tags>
```
