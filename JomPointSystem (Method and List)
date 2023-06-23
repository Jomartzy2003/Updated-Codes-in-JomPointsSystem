using System;
using System.Collections.Generic;

class HelloWorld
{
    static void Main(string[] args)
    {
        JomPointsSystem();
    }
    static void JomPointsSystem()
    {
        int jompoints = 25;

        Console.WriteLine("Welcome to Kuya Joms' Finest Restaurant Loyalty Points System");
        Console.WriteLine("Your balance Jom Points is:" + jompoints);
        Console.WriteLine("______________________________________________________________");
        Console.WriteLine(" ");
        Console.WriteLine("Press 1 to Exchange your Jom Points into BigBoy Prizes");
        Console.WriteLine("Press 2 to exchange your Jom Points into Advantage Card / Ticket");
        Console.WriteLine("Press 3 to Claim more Jom Points");
        Console.WriteLine("Press 4 to Exit the System");
        Console.WriteLine("______________________________________________________________");

        Console.WriteLine("Select what you want?");
        int selectedOption = Convert.ToInt32(Console.ReadLine());
        Console.WriteLine(" Your choice is " + selectedOption);

        while (true)
        {
            if (selectedOption == 1)
            {
                Console.WriteLine(" Select what you wish to exchange?");
                Console.WriteLine("____________________________________________________________");
                Console.WriteLine(" Press 4 for 16 oz of Milk Shake");
                Console.WriteLine(" Press 5 for Plant-Based Burger Steak");
                Console.WriteLine(" Press 6 for Beef-Mushroom Pizza");
                Console.WriteLine("____________________________________________________________");
                Console.WriteLine(" ");
                Console.WriteLine(" Press :");
                int exchangeRewards = Convert.ToInt32(Console.ReadLine());

                List<int> rewardsPoints = new List<int>() { 20, 25, 30 };
                List<string> rewardsNames = new List<string>() { "16 oz of Milk Shake", "Plant-Based Burger Steak", "Beef-Mushroom Pizza" };

                if (exchangeRewards >= 4 && exchangeRewards <= 6)
                {
                    int rewardIndex = exchangeRewards - 4;
                    int rewardPoints = rewardsPoints[rewardIndex];
                    string rewardName = rewardsNames[rewardIndex];

                    if (jompoints >= rewardPoints)
                    {
                        Console.WriteLine(" You've successfully exchange your Jom Points in " + rewardName);
                        jompoints -= rewardPoints;
                        Console.WriteLine(" Your new balance Jom Points is " + jompoints);
                        break;
                    }
                    else
                    {
                        Console.WriteLine(" Not enough Jom Points, earn more");
                    }
                }
                else
                {
                    Console.WriteLine("Invalid reward option selected");
                }
            }

            if (selectedOption == 2)
            {
                Console.WriteLine(" Select what you wish to exchange");
                Console.WriteLine("___________________________________________________________");
                Console.WriteLine(" ");
                Console.WriteLine(" Press 7 for 300-Peso Gift Voucher in any shopping stores");
                Console.WriteLine(" Press 8 for Buy 9 Get 1 Free Card");
                Console.WriteLine(" Press 9 for 1 Million Mega Raffle Draw Ticket");
                Console.WriteLine("___________________________________________________________");
                Console.WriteLine(" ");
                Console.WriteLine("Press :");
                int exchangeRewards = Convert.ToInt32(Console.ReadLine());

                List<int> rewardsPoints = new List<int>() { 30, 30, 15 };
                List<string> rewardsNames = new List<string>() { "300-Peso Gift Voucher", "Buy 9 Get 1 Free Card", "1 Million Mega Raffle Draw Ticket" };

                if (exchangeRewards >= 7 && exchangeRewards <= 9)
                {
                    int rewardIndex = exchangeRewards - 7;
                    int rewardPoints = rewardsPoints[rewardIndex];
                    string rewardName = rewardsNames[rewardIndex];

                    if (jompoints >= rewardPoints)
                    {
                        Console.WriteLine("_______________________________________________________");
                        Console.WriteLine(" ");
                        Console.WriteLine(" Exchange complete, please proceed to the cashier");
                        jompoints -= rewardPoints;
                        Console.WriteLine(" Your new balance Jom Points is " + jompoints);
                        break;
                    }
                    else
                    {
                        Console.WriteLine(" Exchange failed, not enough Jom Points");
                    }
                }
                else
                {
                    Console.WriteLine("Invalid reward option selected");
                }
            }

            if (selectedOption == 3)
            {
                int validCode = 1873293;
                int bonusPoints = 30;
                Console.WriteLine(" Enter the code for additional Jom Points:");
                int enterCode = Convert.ToInt32(Console.ReadLine());
                if (enterCode == validCode)
                {
                    Console.WriteLine("Your submitted code is valid");
                    jompoints += bonusPoints;
                    Console.WriteLine("Your new balance is " + jompoints);
                    break;
                }
                else
                {
                    Console.WriteLine("Invalid code submitted, please try again");
                }
            }

            if (selectedOption == 4)
            {
                Console.WriteLine("_____________________________________________________");
                Console.WriteLine(" Thanks for visiting us, Stay Loyal!!!");
                break;
            }
        }
    }
}
