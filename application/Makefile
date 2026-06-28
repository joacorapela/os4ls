all: application.md

application.md: title.md summary.md expectedValue.md landscape.md workPlan.md goals.md
	echo "# Title (" `wc -c < title.md` "/ 60 words )" > application.md
	cat title.md >> application.md
	echo "\n# Summary (" `wc -c < summary.md` "/ 3000 words)" >> application.md
	echo "\n***Briefly describe the purpose of the proposal and the software project(s) it involves.***\n" >> application.md
	cat summary.md >> application.md
	echo "\n# Expected Value (" `wc -c < expectedValue.md` "/ 1500 words)" >> application.md
	echo "\n***If the proposal is successfully funded, what does success look like? We're seeking to understand: what type of capabilities the proposal is unlocking for the scientific community; how upstream and downstream software will be improved by the proposal; how the proposed work supports or implements novel functionality for AI enablement and large-scale data analysis.***\n" >> application.md
	cat expectedValue.md >> application.md
	echo "\n# Landscape Analysis (" `wc -c < landscape.md` "/ 1500 words)" >> application.md
	echo "\n***We are looking for proposals from software projects with demonstrated traction and adoption. Briefly describe other software tools that the audience for this proposal primarily uses (including proprietary alternatives, if they exist), and how the software project(s) in your proposal compare in terms of user base, adoption, functionality, and maturity relative to their target audience. You can add indicators of adoption and usage as needed. Please indicate if the software is used in AI applications and workflows.***\n" >> application.md
	cat landscape.md >> application.md
	echo "\n# Work Plan (" `wc -c < workPlan.md` "/ 750 words)" >> application.md
	echo "\n***To complete this section, please download or make a copy of the [provided template](https://docs.google.com/document/d/1QeloUWQCiDwTPzZlJQ55tKHAoTHztuhIqSm90aEkuWo/edit?tab=t.0) (by selecting File->Download or File->Make a Copy), complete the required sections, and upload as a single PDF.***\n" >> application.md
	cat workPlan.md >> application.md
	echo "\n# Goals, Outcomes, Milestones and Deliverables (up to 5 goals)\n" >> application.md
	cat goals.md >> application.md
	echo "\n# Budget Description" >> application.md
	echo "\n## Amount Requested" >> application.md
	echo "\nEnter the amount requested in USD per year (whole numbers only) as well as the budget requested for all years. The numbers should match those described in the Budget Description to follow. Please note that for track 1, the maximum amount requested is $250,000 USD  total over two years ($125,000 USD/per year).  For track 2, the maximum amount requested is $1,000,000 total over two years($500,000 USD/per year)." >> application.md
	echo "\nAmount for Year 1: 125000" >> application.md
	echo "\nAmount for Year 2: 125000" >> application.md
	echo "\nTotal Amount: 250000" >> application.md
	echo "\nBudget Description:" >> application.md
	echo "\nUpload the description of the costs to be funded by this grant at a high level in narrative and tabular form, outlining costs for personnel (including names, if known), supplies, equipment, travel, meetings/hackathons/sprints, subcontracts, other costs, and up to 10% indirect costs (excluding equipment and subcontracts). Upload as .pdf and/or .xlsx file formats." >> application.md
	echo "\nBudget Description:" >> application.md
	echo "\nRecent Financial Support ("`wc -c < recentFinancialSupport.md` "/ 1500 words)" >> application.md
	echo "\nList active and recently completed grants (previous two calendar years - 2025 and 2026) as well as in-kind support the PI and any co-PIs have received to directly or indirectly support work related to this proposal, including the software project(s) listed in the proposal, including: their duration, total amount in USD (for grants), and source of funding (maximum 1,500 characters)" >> application.md
	cat recentFinancialSupport.md >> application.md


