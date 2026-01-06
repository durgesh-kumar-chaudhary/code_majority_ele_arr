# code_majority_ele_arr
code for finding majority element in an array
def majorityElement(nums):
    candidate=None
    count=0
    for num in nums:
        if count==0:
            candidate=num
            count=1
        elif num==candidate:
            count+=1
        else:
            count-=1
    return candidate
nums=[2,2,5,2,2,8,2,9]
print(majorityElement(nums))

