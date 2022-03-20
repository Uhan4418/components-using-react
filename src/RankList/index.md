---
nav:
  title: Components
  path: /components

group:
  title: RankList 排行榜
---

## RankList 排行榜

排行榜组件用于简易排行榜业务场景。

**代码示例:**

```tsx
/**
 * title: 基础使用
 * desc: 我是简介，我可以用 `Markdown` 来编写
 */
import React, { FC } from 'react';
import { RankList } from 'components-using-react';

const RankListDemo: FC<any> = () => {
  const data = Array.from(new Array(10)).map((_, idx) => ({
    label: `选项${idx + 1}`,
    value: 10 - idx,
  }));

  return (
    <div>
      <RankList data={data}></RankList>
    </div>
  );
};

export default RankListDemo;
```

<API></API>
