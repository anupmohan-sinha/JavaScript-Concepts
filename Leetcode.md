## A New Post
**Question:-** Input: nums = [2,7,11,15], target = 9
Output: [0,1]
Output: Because nums[0] + nums[1] == 9, we return [0, 1].


var twoSum = function(nums, target) {
    const map = new Map(), len = nums.length;
    for (let i=0; i<len; i++) {
        const complement = target- nums[i];
        if(map.has(complement)) {
            return [i, map.get(complement)];
        }
        map.set(nums[i], i);
    }
};


var twoSum = function(nums, target) {
    let numsObj = {}, len = nums.length;
    for(let index=0; index<len; index++) {
        if(numsObj.hasOwnProperty(target - nums[index])) {
            return [index, numsObj[target - nums[index]]];
        }
        numsObj[nums[index]]= index;
    }
};