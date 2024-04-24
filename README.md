# armstrongnumber
armstrongnumber
bool checkArmstrong(int n){
	//Write your code here
	int m = to_string(n).length();
	int remainNo = n;
	int lastDigit;
	int sum = 0;
	for(int i = 1; i <= m; i++)
	{
		lastDigit = remainNo%10;
		sum += pow(lastDigit, m);
		remainNo /= 10;
	}
	if (sum == n) return true;
	return false;
}
