# mysql 细节( version:5.7.7-rc)

+ null

> mysql中，0和null表示false,其他都为ture.
>
> 不能够使用比较运算符比如 = ，< 或 <> 来比较null
>
> 2个 null 在order by 的语法中是相等的。


1. You cannot use arithmetic comparison operators such as `=`, `<`, or `<>` to test for `NULL`.
2. In MySQL, `0` or `NULL` means false and anything else means true. The default truth value from a boolean
operation is `1`.
3. When doing an `ORDER BY`, `NULL` values are presented first if you do `ORDER BY ... ASC` and last if you
do `ORDER BY ... DESC`.
