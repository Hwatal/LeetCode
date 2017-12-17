# 思路(C++)

好久没登录 LeetCode, 今天一登录，发现 No. 1 的题目都没做。惭愧，而且还是个 Easy 的。
于是决定顺手解决了。

另外，LeetCode 现在有 711 道题了，当初我按照从易到难排序也逐步有些过时了。早知道还不如按照编号顺序来解题呢。这样一天容易一天难的，还挺好玩。

----

这道题有点像找配对。找到 `a`，找到 `b`，让 `a + b = target`。那么肯定得遍历，遍历的过程中，记录什么，成了思考的关键。

既然是配对，那么 kv 结构是非常合适的，于是上了 Hash 表。让 key 就是要找的 `b`，让 value 记录 `a` 的 index，也就是结果需要的索引。

这样思路就很简单明了了。

## Python

基本与 C++ 的思路一致，只不过更简洁了。