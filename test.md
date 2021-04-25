## try to navigate to the README.md

## test
## 跳转
navigate [here](README.md)

![引用自我博客的图片(web)](https://img-blog.csdnimg.cn/20210425143046399.jpg?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L20wXzQ4Nzc1MzE5,size_16,color_FFFFFF,t_70#pic_center)

## 本地的图片(我的青春恋爱物语果然有问题的女主角)
![local pic](YoukiNa.png)


## 另外，欢迎老师访问我的博客(a link to an external website)
click [here](http://mingyangovo.gitee.io/liumingyang/)

## 这是一个二级标题 This is H2 sized Title

#### This is a h4 sized Title

#### 有关代码块，以下是最近练习的有路径压缩优化的并查集板子
```cpp
class Djset
{
    public:
        vector<int> parent;	//
        vector<int> rank;	//深度
        Djset(int n): parent(vector<int>(n)), rank(vector<int>(n))
        {
            for (int i = 0; i < n; ++i) {parent[i] = i;}
        }
        int find(int x)
        {
            if (parent[x] != x) {parent[x] = find(parent[x]);}
            return parent[x];
        }
        void merge(int x, int y)
        {
            int rootx = find(x);
            int rooty = find(y);
            if (parent[rootx] != parent[rooty]) 
            {
                if (rank[x] < rank[y]) {swap(rootx, rooty);}
                parent[rooty] = rootx;
                if (rank[rootx] == rank[rooty]) {rank[rootx] += 1;}
            }
        }
};
```
#### 有关斜体文本
*This is a test! Let's learn Disjoint Set*

#### 有关表格

|  姓名   | 是否爱吃芒果  |
|  ----  | ----  |
| 刘铭扬  | 爱吃 |
| 老师  | 不知道 |
#### 有关删除线
~~我喜欢学英语，我热爱编程~~ 

#### 有关粗体字
**你好，我是粗体字**

#### 有关引用
> 这里是引用：难忍覆余觞，临风泪数行


#### 有关有序表
 1. 我要完成github的作业
 2. 我要重新做一遍错题
 3. 我要吃掉宿舍里的甜瓜
 4. 我要好好睡一觉