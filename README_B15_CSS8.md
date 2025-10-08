# BỘ CHỌN

## 2.3 Bộ chọn

### 2.3.1 Các loại bộ chọn

- Bộ chọn cơ bản (basic selector).
- Bộ chọn gộp (grouping selector).
- Bộ chọn tổ hợp (combinator).
- Bộ chọn theo trạng thái (pseudo-class, pseudo-element).

**Bộ chọn cơ bản**

|**Bộ chọn**|**Cú pháp**|
|-----------|-----------|
|Bộ chọn phổ quát (universal selector): chọn mọi phần tử| `* {}` ` ns \| * {}` `* \| * {}`|
|Bộ chọn theo tên phần tử (type selector, element selector): chọn các phần tử theo tên.|`elementname {}`|
|Bộ chọn theo class: chọn các phần tử theo giá trị của thuộc tính class|`.classname{}`|
|Bộ chọn theo ID: chọn phần tử theo giá trị của thuộc tính ID|`#idname{}`|
|Bộ chọn theo thuộc tính (attribute): chọn các phần tử theo tên, hoặc giá trị của thuộc tính|`[attr]  [attr=value]  [attr~=value]  [attr\|=value]  [attr^=value]  [attr$=value] [attr*=value]`|
