# reto_piggy
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApplication1
{
    class pigggybank
    {
        private decimal m_bankbalance;
        public event BalanceEventHandler balanceChanged;
        public decimal theBalance {
            set
            {
                m_bankbalance = value;
                balanceChanged(value);
            }
            get
            {
                return m_bankbalance;
            }
        }
    }
    class Program
    {
        static void Main(string[] args)
        {
            pigggybank pb = new pigggybank();

            pb.balanceChanged += (amount) => Console.WriteLine("")
            pb.balanceChanged += (amount) => { if (amount>500.0m)}

            string theStr;
            do
            {
                console.writeline("how much to deposit?");

            }
        }
    }
}
