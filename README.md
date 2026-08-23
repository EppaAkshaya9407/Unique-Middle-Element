# Unique-Middle-Element
Class Solution:
    def isMiddleElementUnique(self, nums: list[int]) -> bool:
        n=len(nums)
        r=n//2
        mid=nums[r]
        c=0
        for i in range(n):
            if mid==nums[i]:
                c+=1
        if c>1:
            return False
        return True
