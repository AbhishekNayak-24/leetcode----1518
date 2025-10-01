# leetcode----1518
Water Bottles
//code in GO
func numWaterBottles(numBottles int, numExchange int) int {
    if numExchange <= 1 {
        return 1<<31 - 1
    }
    return numBottles + (numBottles-1)/(numExchange-1)
}
