## 函数作用
1.pop_back()	删除 vector 容器中最后一个元素，该容器的大小（size）会减 1，但容量（capacity）不会发生改变。

2.erase(iter)	删除 vector 容器中iter迭代器指定位置处的元素，并返回指向被删除元素下一个位置元素的迭代器。该容器的大小（size）会减 1，但容量（capacity）不会发生改变。

3.erase(iter1，iter2)	删除 vector 容器中位于迭代器 (iter1,iter2)指定区域内的所有元素，并返回指向被删除区域下一个位置元素的迭代器。该容器的大小（size）会减小，但容量（capacity）不会发生改变。

4.clear()	删除 vector 容器中所有的元素，使其变成空的 vector 容器。该函数会改变 vector 的大小（变为 0），但不是改变其容量。

5.remove(iter1，iter2，key)	删除容器中所有和指定元素值相等的元素，并返回指向最后一个元素下一个位置的迭代器。值得一提的是，调用该函数不会改变容器的大小和容量。（后面会详细说明，该函数的用法）

6.swap(vector)	用于交换向量的内容，用一个向量调用它并接受另一个向量作为参数并交换它们的内容。 (两个向量的大小可能不同)。通过交换向量进行删除。

7.shrink_to_fit()	将vector 容器的容量缩减至和实际存储元素的个数相等。可以配合以上的函数，收回内存