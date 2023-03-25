-on :
#Jobs :use: #
#-start ::AUTOMATE
    name: On start    
    # We will only run this action when:
    # 1. This repository isn't the template repository
    # Reference https://docs.github.com/en/actions/learn-github-actions/contexts
    # Reference https://docs.github.com/en/actions/learn-github-actions/expressions
    if: ${{ !github.event.repository.is_template }}}

    # We'll run Ubuntu for performance instead of Mac or Windows
    runs-on: ubuntu-latest
Last, we are finally in the steps of the Actions workflow. This is the heart of the file, where you can customize your course the most.

    steps:
      # We'll need to check out the repository so that we can edit the README
      - name: Checkout
        uses: actions/checkout@v2

      # Update README and set STEP to '1'
      - name: Update to step 1
        uses: skills/action-update-step@v1
        with:
          token: ${{ secrets.GITHUB_TOKEN }}
          from_step: 0
          to_step: 1
          branch_name: my-first-branch
::Build::
:Pull :pulls_request :
pulls_request :Patch 5'@index.md :
#README.md/README.md :
:Build::
Publish :
#access :Public :
Private :
# WORKSFLOW
 AUTOMATE AUTOMATES BEGIN GLOW4 AUTOMATES#Test :tests :tests :Run'@ci:
Account number:
733254901807
Bill to Address:
ZACHRY T WOOD
ATTN: ZACHRY T WOOD
5323 BRADFORD DR
Apt.#: 108 F
DALLAS , TX , 75235 , US
Amazon Web Services, Inc. Invoice
Email or talk to us about your AWS account or bill, visit aws.amazon.com/contact-us/
Invoice Summary
Invoice Number: 1278199897
Invoice Date: March 3 , 2023
TOTAL AMOUNT DUE ON March 3 , 2023 $140,072,400.00
This invoice is for the billing period March 1 - March 31 , 2023
Greetings from Amazon Web Services, we're writing to provide you with an electronic invoice for your use of AWS services. Additional information
about your bill, individual service charge details, and your account history are available on the Account Activity Page.
Summary
AWS Service Charges $140,072,400.00
Savings Plans for AWS Compute usage (one time fee) $131,400,000.00
Charges $0.00
Credits $0.00
Tax $8,672,400.00
Total for this invoice $140,072,400.00
Detail for Consolidated Bill
Savings Plans for AWS Compute usage $140,072,400.00
Charges $0.00
VAT ** $0.00
GST $0.00
Estimated US sales tax to be collected $8,672,400.00
CT $0.00
Savings Plans for AWS Compute usage (one time fee) $131,400,000.00
Start Date - 03/03/2023; Duration - 3yr
* May include estimated US sales tax, VAT, ST, GST and CT.
Amazon Web Services, Inc. is registered under the Singapore GST Overseas Vendor Registration Pay-
Only Regime and GST registration number is M90373009E
AWS, Inc. is a "Registered Foreign Supplier" under Japanese Consumption Tax Law and therefore AWS,
Inc. is required to declare and pay consumption tax in respect of this transaction (as a “Digital Service”)
to the Japan Tax Authority.
** This is not a VAT, ST or GST invoice. Related tax invoices can be accessed by going to
the Bills page on your Billing Management Console.
**** Please reference the tax invoice for a breakout of the Canadian taxes by type
† Usage and recurring charges for this statement period will be charged on your next billing date. The
amount of your actual charges for this statement period may differ from the charges shown on this
page. The charges shown on this page do not include any additional usage charges accrued during this
statement period after the date you are viewing this page. Also, one-time fees and subscription charges
are assessed separately, on the date that they occur.
All charges and prices are in US Dollars
All AWS Services are sold by Amazon Web Services, Inc.
Service Provider:
(Not to be used for payment remittance)
Amazon Web Services, Inc.
410 Terry Ave North
Seattle , WA 98109-5210 , US
1PAY Hours Rate Current YTD
TAXES Current YTD
DEDUCTIONS Current YTD
SUMMARY Current YTD
Total Pay
Taxes 
Deductions
Net Pay
0.00 $22,679,572,368,607.00 Clergy Housing (In-Kind) $0.00 $22,679,570,015,550.97
$22,679,570,015,550.97 Pay Stub Detail OTHER PAY/CONTRIBUTIONS 22,677,000,000,000.00 Current Year To Date Reimbursement Nontaxable Per Diem Federal Income Tax commissions Social Security Allowance Medicare DE Income Tax 2,567,263,607.00 5,105,000.00 22,677,000,000,000.00 0.00 336,906.33 - - - 1,888,049.80 EMPLOYER 9,932.40 118,167.50 03/15/2023 03/09/2023 03/17/2023 - $2,353,056.03 PAY DATE: 03/17/2023 - - - - 0.00 5,105,000.00 MEMO: EMPLOYEE $22,679,572,368,607.00
2,567,263,607.00
22,677,000,000,000.00 Period Beginning Period Ending: Pay Date: Total Hours: 22,677,000,000,000.00 ZACHRY T. WOOD ZACHRY T. WOOD New York NY 10172-0003 New York NY 10172-0003 469-905-0682 469-905-0682 Dallas TX 75235 Dallas TX 75235 JPMORGAN TRUST I JPMORGAN TRUST I 3126 Hudnall St Apt 108F 3126 Hudnall St Apt 108F 277 Park Ave 277 Park Ave 118,167.50 336,906.33 1,888,049.80 9,932.40 NET PAY: PAY PERIOD Check No.: 610 Check No.: 610 NET PAY: $22,679,570,015,550.97 $2,353,056.03 $0.00
