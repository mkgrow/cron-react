---
nav:
  title: Cron表达式
  path: /cron
group:
  title: 其他
---

## Cron 组件

根据选择的类型和时间生成cron表达式

```tsx
import React, { useState } from 'react';
import { Space } from 'antd';
import Cron from 'react-cron-cn';

export default () => {
  const [value, setValue] = useState(null);
  
  return (
    <Space direction='vertical' style={{width: '100%'}}>
      <Cron defaultType='customize' value={value} onChange={setValue} />
      <div>{value}</div>
    </Space>
  )
};
```

<API src="./index.tsx" ></API>
