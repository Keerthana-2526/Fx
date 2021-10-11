# Fx
public class FXCalculation {
	//1 USD=73.65 Rupees;
	 static double USD=73.65;
	 public static double converter(long RupeesAmount) {
		 return(RupeesAmount *100/7365);
	 }

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		long RupeesAmount=1000000;
		double USD_Amount=converter(RupeesAmount);
		double Profit=50;
		double Total_Amount=USD_Amount+Profit;
		/*
		 * markup %=(Selling price-cost)/cost*100
		 */
		double Exchange_Rate=((Total_Amount-USD_Amount)/USD_Amount*100);
		System.out.println("Amount inRs==>"+" Rs"+RupeesAmount);
		System.out.println("Exchange Rate==> "+String.format("%2f", Exchange_Rate));
		System.out.println("Profit in $==>"+" $"+Profit);
		System.out.println("Amount to be paid by customer($)==>"+" $"+String.format("%.2f", Total_Amount));
		

	}

}
