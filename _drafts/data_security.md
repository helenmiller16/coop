Susan Glick as author

- Does not address remote security or security in the era of Covid.
- links are internal, should be noted
- include links to public sites with relevant info?

Landing squarely at the feet of the Hutch Integrated Data and Archives (HIDRA) project, I soon understood the textured value of data.  Data generation, capture, curation and computation is at once the vessel and lifeblood of research.  Data generation and curation is pushed by the confluence of improved capabilities of Next Generation Sequencing, Electronic Health Records, and Open Science.  Analysis rests on the strength of computational abilities, including scripting and coding.  In essence, it is the ability to master the dynamic ramification and convergence of multiple data streams that pushes information to medical discovery.

However, in the shadows of rapid data exploration and computational pipelines stands safeguarding the flow of sensitive data.  Salient privacy and security challenges not fully addressed by regulatory agencies (e.g., de-identification of genomic data or knitting such information into a patient’s medical record) leaves individual institutions at the local front of security and privacy guidance.  Researchers often try to navigate with marginal experience or resources how to be ethical, compliant and secure.

Being ethical, compliant and secure starts at the beginning with a data management plan, many examples of which can be found at the NIH or DMP.  A primary key to a good plan is to know just how sensitive your data is.  Is the data generated through research or extracted from an EHR or direct care provider? Is the research likely to be shared within a multisite effort or collaboration?  DMP components such as password management, data gatekeeping processes, account authorization policies can be scaled to match the information’s sensitivity.  Yet, once you have solidified your plan and levied expectations to use it, all too often ongoing awareness remains a silent witness. And, incidents and accidents do happen.

Perhaps reviewing a list of what has actually happened will provide some insight into how to avoid incident creep.  Because, honestly, incidents tend to happen where DMPs don’t reach.

GitHub, GitLab or Git”X” is a love-meh relationship.  A favorite for code and data analysis versioning and sharing, Git”X” doesn’t care whether your coding or markdown contains sensitive information.  For that reason, sensitive data, human or not, does not belong in a multiple-party, open, sharing environment.  Also, a more-than-once occurrence is scripting AWS credentials, or any account credentials, into a Git”X” repository.  In one instance, within a few minutes of finding the credentials, a trolling bot/program accessed a FH account and used FH resources to mine for cryptocurrency.  Over $1,000 of compute charges accrued to FH, but no sensitive data breached.

Misconfiguring a server, cloud database, storage container, or search engine is one of the most common errors resulting in security incidents.  Vulnerabilities leading to access may be exploited on machines which do not have sufficient endpoint security, may be running older operating systems or are not patched.  Leaky AWS S3 buckets are a common soft spot.  An example: a database specific to a protocol within REDCap was lingering with DBA responsibilities shifting between individuals.  After various revisions, a misconfiguration allowed Google to index the database information, opening data to the public through Google search. The breach exposed the ability re-identify participant-donors.

The “One-off Activity” not only breaks the routine, but also the compliance mindset.  The “one-off” is a time to be most vigil.  Two incidents related to a “one-off” help explain this.  First, a research project was moving data via Dropbox to support a research-related, one-time event. The person using drop-box was a more peripheral member of the research team. The Dropbox account was not secure and recipients included individuals not authorized to the research.  An unauthorized individual recognized a family member as a research subject.  Second, a collaboration using medical record information conducted a proof of concept visualization for a presentation with the data; the application used to develop the visualization was misconfigured to be open to the public.  The medical records of 11 individuals was public for over 9 months.

Training the expert is important.  Many researchers learn computation methods or scripting on the side, using a brew of Python or R to move and transform data.  Conversely, labs will hire from private industry, but lag to educate the expert software developer on compliance and security regulation in healthcare and research.  Fred Hutch is slowly moving to improve training offerings; the revised security and confidentiality training is an excellent start.

De-Identification is more than just anonymizing a name.  In a Dropbox incident, a recipient was able to use age, census tract of home address, date of encounter, race, and location of enrollment to identify a research subject.  Small cell sizes can also lead to re-identification. Learn more about de-identification at [HDC Data Requests, Data Compliance, Data Security](https://centernet.fredhutch.org/cn/u/hdc/compliance---governance.html).

The Open Source alternative may be more development-intensive than it appears.  If you adopt or adapt open source products to be used with sensitive data, the application must adhere to FH Information Security Policy and Standards, in such areas as audit and identity management.  The standards are found here: [ISO Policies and Standards Program](https://centernet.fredhutch.org/cn/u/center-it/iso/iso-policy---standards-program.html).  You can use the [Information Classification and Handling Standard](https://teams.fhcrc.org/sites/centerit/governance/PSP/FinalDocs/Fred-Hutch-Information-Classification-and-Handling-Standard%20-%20Final%20v2.pdf) to determine your data sensitivity.

Whether computational research or experimental, research ethics, compliance and security morph in parallel with the evolving technology which powers analysis and computation.  Datasets are bigger so single breach incidents have more risk. Emerging methods and technologies to de-identify human data are unfamiliar to IRBs, creating delays.  Open science means matching the sensitivity of your information to the governance structure of the selected third-party repository.  Data transport between collaborators is all too often not considered a pressure point.  The research lab’s data pipeline with multiple linkages needs audit capability.  These may not be traditional factors of privacy and security, but they may become so as the discipline advances to be more data driven.