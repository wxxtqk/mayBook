# svg作为背景图

在平时我们做背景图的时候，一般都是用图片，但是有时候UI给的会是svg,用svg做背景图可能会遇到一些问题,比如设置background-size无效，有时候我们会发现background-size: 100% 100%,并不能够把dom元素充满，只要设置preserveAspectRatio属性，preserveAspectRatio表示是否强制进行统一缩放，preserveAspectRatio只适用于在同一元素上为 `viewBox` 提供的值。对于这些元素，如果没有提供属性 `viewBox` ，则忽略了preserveAspectRatio。

```html
<?xml version="1.0" encoding="UTF-8"?>
<svg width="17px" height="20px" viewBox="0 0 17 20" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" preserveAspectRatio="none meet">
    <!-- Generator: Sketch 56.3 (81716) - https://sketch.com -->
    <title>第三名背景</title>
    <desc>Created with Sketch.</desc>
    <g id="页面-1" stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
        <g id="涉稳-首页备份-13" transform="translate(-1356.000000, -237.000000)" fill="#44D7B6">
            <g id="分组-15-copy-2" transform="translate(1356.000000, 229.000000)">
                <polygon id="第三名背景" points="0 8 17 8 17 28 8.5 25.049728 0 28"></polygon>
            </g>
        </g>
    </g>
</svg>
```

详情参考preserveAspectRatio属性值