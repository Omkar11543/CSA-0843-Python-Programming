def maxProfit(price, a):	
	profit = [0]*a
	max_price = price[a-1]
	for i in range(a-2, 0, -1):
		if price[i] > max_price:
			max_price = price[i]		
		profit[i] = max(profit[i+1], max_price - price[i])	
	min_price = price[0]
	for i in range(1, a):
		if price[i] < min_price:
			min_price = price[i]
		profit[i] = max(profit[i-1], profit[i]+(price[i]-min_price))
	result = profit[a-1]
	return result
price = [2,30,15,10,8,25,80]
print ("Max profit is", maxProfit(price, len(price)))
