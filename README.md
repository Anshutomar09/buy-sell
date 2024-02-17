# buy-sell

class Solution {
public:
    int maxProfit(vector<int>& prices) {
        int n=prices.size(),min=prices[0],i=1,profit=0;
        while(i<n){
            if(prices[i]<min){
                min=prices[i];
            }
            else{
                profit=max(profit, prices[i]-min);
            }
            
i++;
            }
        return profit;
    }
};
