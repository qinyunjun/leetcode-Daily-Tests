# leetcode Daily Tests (2022/11/30)

### toc:

[toc]

### related links:

[895. Leetcode](https://leetcode.cn/problems/maximum-frequency-stack/solutions/1997251/zui-da-pin-lu-zhan-by-leetcode-solution-moay/)

[Swoole HashMap zhihu.com](https://zhuanlan.zhihu.com/p/45020990#:~:text=UT_hash_handle 是存储数据的真正地方，也是哈希表的最小结构单元，如下图，不同于一般的开链法，只有在哈希冲突的时候才会将两个元素用链表连接起来，uthash,哈希表将所有 UT_hash_handle 元素构成了两种双向链表)

[C Structures (structs) (w3schools.com)](https://www.w3schools.com/c/c_structs.php)

[Structures in C - GeeksforGeeks](https://www.geeksforgeeks.org/structures-c/)

## node / structure defined

（Weak foundation aaaa~）：

### structure data type：

![Data-types-in-C](https://yunjunqin.oss-cn-beijing.aliyuncs.com/Data-types-in-C.png)

```
structures belong to derived DT.
```

### structures (structs) define:

Structures (also called structs)

1.a way to group several related variables into one place

2.Each variable in the structure is known as a **member** of the structure.

Compare it to an array of the same level:

1.can contain many different data types (int, float, char, etc.).

### structure creation:

![img](https://media.geeksforgeeks.org/wp-content/cdn-uploads/Structure-In-C.png)

```c
struct address
{
char name[50];
char street[100];
char city[50];
char state[20];
int pin;
};
```

#### structure variables declaration:

1.be declared with structure declaration

```c
// A variable declaration with structure declaration.
struct Point
{
   int x, y;
} p1;  // The variable p1 is declared with 'Point'
```

2.be declared as a separate declaration like basic types. 

```c
// A variable declaration like basic data types
struct Point
{
   int x, y;
};
 
int main()
{
   struct Point p1;  // The variable p1 is declared like a normal variable
}
```

```
Note: In C++, the struct keyword is optional before in declaration of a variable. In C, it is mandatory.
```

#### structure members initialization

1.Structure members cannot be initialized with declaration
2.Structure members only can be declared.

```c
struct Point
{
   int x = 0;  // COMPILER ERROR:  cannot initialize members here
   int y = 0;  // COMPILER ERROR:  cannot initialize members here
};
```

```c
struct Point
{
   int x, y;
};
 
int main()
{
   // A valid initialization. 
   //member x gets value 0 and y gets value 1.  
   //The order of declaration is followed.
   struct Point p1 = {0, 1};
}
```

##### (add: How memory is allocated when a data structure is declared)

[How memory is allocated when a data structure ... | DaniWeb](https://www.daniweb.com/programming/software-development/threads/463769/how-memory-is-allocated-when-a-data-structure-is-declared)

