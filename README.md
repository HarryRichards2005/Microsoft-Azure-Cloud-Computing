
<p>"Paws & Whiskers" is a growing pet shop that aims to improve its business by analysing sales, customer information, and inventory data. Currently, the data is collected manually or stored in spreadsheets. Management is interested in transitioning to Microsoft Azure to streamline data storage, analysis, and reporting, enabling them to make data-driven decisions.</p>
<p>Data Laws and Regulations:</p>
<p>&ldquo;Paws and Whiskers&rdquo; need to ensure that they handle their customers data responsibly. This is because it ensures they maintain their reputation and their customers trust additionally to be legally compliant. The biggest example of this is GDPR which state how data should be collected, stored, and processed. It allows customers to be in control of their personal information, Paws and Whiskers will be collecting clients online account information, and customer names. GDPR has seven key principles that must be followed, these are</p>
<ul>
<li>Lawfulness, Fairness, and Transparency
<ul>
<li>Data must be processed legally; customers must know how their data is being used.</li>
</ul>
</li>
<li>Purpose Limitation
<ul>
<li>Data should only be collected for a specific purpose.</li>
</ul>
</li>
<li>Data Minimisation
<ul>
<li>Only the necessary amount of data should be collected.</li>
</ul>
</li>
<li>Accuracy
<ul>
<li>Data must be accurate and up to date.</li>
</ul>
</li>
<li>Storage Limitation
<ul>
<li>Data should not be kept longer than needed.</li>
</ul>
</li>
<li>Integrity &amp; Confidentiality
<ul>
<li>Data must be kept safe and secure from unauthorised breaches.</li>
</ul>
</li>
<li>Accountability
<ul>
<li>Paws and Whiskers must be able to prove they are following this legislation.</li>
</ul>
</li>
</ul>
<p>Another prominent piece of legislation Paws and Whiskers will have to comply with is the Data Protection Act 2018. The Data Protection Act implements GDPR into UK law as a result it also aims to implement privacy and ensure data is collected, stored, and handled responsibly. Much like GDPR. The Data Protection Act explores four key areas</p>
<ul>
<li>General Data Processing</li>
<li>Law Enforcement Processing</li>
<li>Intelligence Services Processing</li>
<li>Regulation and Enforcement</li>
</ul>
<p>This affects Paws and Whiskers because they need to ensure that their reasons for processing data align with the standards of this legislation. For example, how the customer consent is obtained and recorded, how securely has the personal data been stored, and their rights to access their data or have it deleted.</p>
<p>Additional industry standards might include Payment Card Industry Data Security Standard (PCI DSS). If they process cards payments protects customers against potential misuse of their personal information. Such as, credit/debit card numbers, expiration dates and security codes. The standard&rsquo;s security controls help business minimise the risk of data breaches.</p>
<p>Azure Service Recommendations:</p>
<p>Microsoft Azure offers a range of services suitable for Paws and Whiskers needs to store, analyse, and manage data effectively.</p>
<p>Data Storage</p>
<ul>
<li>Blob Storage
<ul>
<li>Ideal for storing massive volumes of unstructured data. This could be ideal for transaction logs. Its good because its scalable, simple, and cost effective. It provides built-in encryption and there are multiple blob types so they can easily match their workload requirements.</li>
</ul>
</li>
<li>Azure SQL Database
<ul>
<li>This is a relational database best suited for storing customer records and inventory lists. It includes high scalability and performance. It enables them to take advantage of the clouds flexibility and efficiency to scale their database on demand so they only must pay for the resources that they use.</li>
</ul>
</li>
</ul>
<p>Data Analysis Tools</p>
<ul>
<li>Azure Machine Learning
<ul>
<li>Can be used to predict purchasing trends or customer behaviour.</li>
</ul>
</li>
<li>Azure Synapse Analytics
<ul>
<li>Ideal for analysing large data sets such as product performance.</li>
</ul>
</li>
</ul>
<p>Data Integration and Automation</p>
<ul>
<li>Azure Data Factory
<ul>
<li>Azure Data Factory can help to automate their processes by using automated data extraction and transformation. It can gather data from online sales platforms or inventory systems into a single data store. Automating the process and mitigating risk of human error.</li>
</ul>
</li>
</ul>
<p>Data Types and Data Modelling</p>
<ul>
<li>Data Categories
<ul>
<li>Customer demographics &ndash; what is their name, email address, phone number. What is their age and where do they reside.</li>
<li>Transaction data &ndash; what is their purchase history, common trends in their spending habits.</li>
<li>Pet inventory &ndash; what types of animals will they stock, what specific care needs will the customer need to know and what will the length of ownership be.</li>
<li>Product Categories &ndash; group the animals by type. Identify other products like food, toys, treats.</li>
</ul>
</li>
<li>Data Modelling Approach
<ul>
<li>A relational data model is best since this data is structured and can be stored in a tabular format.</li>
<li>They would need tables such as Customers, Orders, and Inventory</li>
<li>This data model would need primary keys (unique identifiers) and foreign keys (primary keys present in other tables) so they can define relationships between tables.</li>
<li>Customer data &ndash; customer id, first name, last name, phone number</li>
<li>Transaction data &ndash; transaction id, items bought, purchase date, customer id, inventory id</li>
<li>Inventory data &ndash; inventory id, stock levels, pricing</li>
<li>In this case, three tables all contain a primary key and there are two foreign keys found in the transaction data table. This defines the relationships between these table allowing for insights and analysis. For example, the primary key in the customer data table can also be found as a foreign key in the transaction data table.</li>
<li>For analysis a star schema can be used.
<ul>
<li>Fact tables for transaction data</li>
<li>Dimension tables for inventory and customer data</li>
</ul>
</li>
</ul>
</li>
</ul>
<p>Data Storage Formats and Structures in Azure:</p>
<ul>
<li>Data Formats
<ul>
<li>CSV is suitable for raw data imports from tills or third-party systems. Very easy to read and write, it becomes less effective with bigger files.</li>
<li>JSON is ideal for semi-structured data such as API responses or web data.</li>
<li>Parquet is recommended for analytics in Azure Synapse due to it compressed, column-based format, which improves performance.</li>
</ul>
</li>
<li>Data Security and Encryption
<ul>
<li>They can secure data by enabling the Azure default encryption-at-rest.</li>
<li>They can implement Role-Based Access Control to limit data access, though it is important that data can still be accessed to ensure compliance with data privacy regulations.</li>
<li>They can also achieve this by utilising Microsoft defender for cloud for continuous monitoring, threat detection, and receive security recommendations.</li>
<li>They can also use Microsoft Purview to identify, classify, and protect sensitive data.</li>
</ul>
</li>
</ul>
<p>Additional Considerations</p>
<ul>
<li>Backup and Disaster Recovery
<ul>
<li>Azure backup can provide automated backups of databases and storage accounts.</li>
<li>Azure site recovery ensures can ensure continuity by replicating data to secondary locations in the event of a system failure.</li>
</ul>
</li>
<li>Data Visualisation
<ul>
<li>Power BI can be integrated with Azure SQL database and Synapse analytics to create dashboards that could show
<ul>
<li>Sales performance</li>
<li>Best-selling products</li>
<li>Customer purchasing trends</li>
</ul>
</li>
<li>Providing Paws and Whiskers with real-time insights in which they can make informed decisions from.</li>
</ul>
</li>
</ul>
