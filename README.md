# LikeDislike
LikeDislike problem from Hackerrank

Question :
There is an array of  integers. There are also  disjoint sets,  and , each containing  integers. You like all the integers in set  and dislike all the integers in set . Your initial happiness is . For each  integer in the array, if , you add  to your happiness. If , you add  to your happiness. Otherwise, your happiness does not change. Output your final happiness at the end.

#Code
_ = input()
array = input().split()
like = set(input().split())
dislike = set(input().split())
print(sum((i in like) - (i in dislike) for i in array))


