## **Cấu trúc của FlexBox**

![syntax](https://images.viblo.asia/0c116fbb-972d-4162-8506-bac8605cd704.png)

1. `display`: đặt ở phần tử cha để áp dụng flexbox

```css
.container {
  display: flex;
}
```

2. `flex-direction`: chỉ định hướng hiển thị của các item

_Lưu ý: Chiều hiển thị mặc định sẽ là từ trái -> phải, từ trên -> dưới_

- row (default): left to right
- row-reverse: right to left
- column: same as row, but top to bottom
- column-reverse: same as row-reverse but bottom to top

3. `flex-wrap`:

Mặc định các flex-item sẽ cố gắng nằm vừa trên 1 dòng

- nowrap (default): tất cả phần tử đều nằm trên cùng 1 dòng
- wrap: các phần tử sẽ xuống dòng theo chiều (top -> bottom)
- wrap-reverse: các phần tử sẽ xuống dòng theo chiều (bottom -> top)

4. `flex-flow`: Cách viết tắt của `flex-direction` và `flex-wrap`:
   default: row nowrap

```css
.container {
  flex-flow: column wrap;
}
```

5. `justify-content`: tùy chỉnh linh hoạt khoảng trống theo trục main

- flex-start (default): các items sẽ được đồn về phía start của flex-direction.
- flex-end: các items sẽ được đồn về phía end của flex-direction.
- center: các items sẽ được căn giữa theo trục main
- space-between: Các items được phân bổ đều, bắt đầu ở đầu trục và kết thúc ở cuối trục
- space-around: Các items được phân bổ đều với khoảng cách xung quanh chúng bằng nhau
- space-evenly: Các items được phân bổ sao cho khoảng cách giữa nó đến các cạnh gần chúng bằng nhau

6. `align-items`:

- stretch (default): kéo dài để lấp đầy container
- flex-start:
- flex-end:
- center: icác items sẽ được căn giữa theo trục cross

7. `align-content`: tùy chỉnh linh hoạt khoảng trống theo trục cross

- normal (default):
- flex-start / start: các items sẽ được dồn về phía start của flex-direction.
- flex-end / end: các items sẽ được đồn về phía end của flex-direction.
- center:
- space-between:
- space-around:
- space-evenly:
- stretch: kéo dài để chiếm hết không gian còn lại

8. `gap`, `row-gap`, `column-gap`

```css
.container {
  display: flex;
  ...
  gap: 10px;
  gap: 10px 20px; /* row-gap column gap */
  row-gap: 10px;
  column-gap: 20px;
}
```

9. `order`: Kiểm soát thứ tự xuất hiện của các items
10. `flex-grow`:
11. `flex-shrink`:

_Lưu ý: Số âm không hợp lệ_

12. `flex-basis`:

13. flex: là cú pháp shorthand của flex-grow, flex-shrink and flex-basis

```css
.item {
  flex: none | [ < "flex-grow" > < "flex-shrink" >? || < "flex-basis" >];
}
```

## **Game**

https://flexboxfroggy.com/#vi
