<h1>Library Management System - Web Application</h1>

<p>
    This project is a <strong>Library Management System</strong> developed as a web application using <strong>Java</strong> and <strong>Servlets</strong> with a <strong>PostgreSQL</strong> database backend.
    The application allows librarians and library members to perform various tasks such as searching for documents, borrowing and returning documents, managing document information, and handling overdue fines.
</p>

<h2>Table of Contents</h2>
<ul>
    <li><a href="#features">Features</a></li>
    <li><a href="#document-types">Document Types</a></li>
    <li><a href="#user-roles">User Roles</a></li>
    <li><a href="#database-structure">Database Structure</a></li>
    <li><a href="#installation">Installation</a></li>
    <li><a href="#usage">Usage</a></li>
</ul>

<h2 id="features">Features</h2>

<h3>For Members:</h3>
<ul>
    <li><strong>Search Documents</strong>: Members can search the library's catalog for documents.</li>
    <li><strong>Borrow Documents</strong>: Members can borrow copies of documents (e.g., books, journals, magazines) for a set time period (e.g., 2 weeks).</li>
    <li><strong>Return Documents</strong>: Members can return borrowed documents and avoid late fines.</li>
    <li><strong>Overdue Fines</strong>: Members are fined if a borrowed document is not returned by the due date.</li>
    <li><strong>Saved Searches</strong>: Members can store and re-execute their previous searches for easier document access.</li>
</ul>

<h3>For Librarians:</h3>
<ul>
    <li><strong>Search Documents</strong>: Librarians can search the library's catalog.</li>
    <li><strong>Manage Users</strong>: Librarians can manage members and their access, including adding and removing members.</li>
    <li><strong>Manage Documents</strong>: Librarians can add, delete, or modify information about documents and their copies.</li>
    <li><strong>Check Overdue Documents</strong>: Librarians can track overdue documents and notify members about fines.</li>
</ul>

<h2 id="document-types">Document Types</h2>

<p>The library system manages several types of documents, each having distinct attributes:</p>

<h3>Books</h3>
<ul>
    <li>Written by one or more authors.</li>
    <li>Published by a publisher.</li>
    <li>Can have multiple editions, each published in a certain year.</li>
    <li>Example: <em>Database System Concepts, 7th edition</em> (2020), by Silberschatz, Korth, and Sudarshan.</li>
</ul>

<h3>Journal Articles</h3>
<ul>
    <li>Written by one or more authors.</li>
    <li>Published in a journal, which has periodic issues.</li>
    <li>Each journal issue has editors and a publication date.</li>
    <li>Example: <em>Antibody Therapeutics in Cancer</em> published in the <em>13 September 2013</em> issue of <em>Science</em> journal.</li>
</ul>

<h3>Magazines</h3>
<ul>
    <li>Published periodically, with each issue having its own title, contributors, and editors.</li>
    <li>Example: <em>National Geographic</em>, December 2020 issue.</li>
</ul>

<h3>Theses and Technical Reports</h3>
<ul>
    <li>Documents like student theses or institutional technical reports, often associated with academic research.</li>
</ul>

<h3>Document Copies</h3>
<p>
    Each document may have multiple physical or digital copies in the library. Copies are stored in specific locations (rooms, levels, etc.). 
    Information about each copy includes whether it is borrowed and, if so, by whom.
</p>

<h2 id="user-roles">User Roles</h2>

<p>The system supports two main roles:</p>

<h3>1. Members:</h3>
<ul>
    <li>Can search for documents.</li>
    <li>Can borrow and return documents.</li>
    <li>Must return borrowed documents within a set period (e.g., 2 weeks).</li>
    <li>Can save searches for future use.</li>
</ul>

<h3>2. Librarians:</h3>
<ul>
    <li>Can perform all actions that members can.</li>
    <li>Can add, delete, or modify document information.</li>
    <li>Can manage user accounts (members).</li>
    <li>Can check for overdue documents and handle fines.</li>
</ul>

<h2 id="installation">Installation</h2>

<h3>Prerequisites</h3>
<ul>
    <li>Java Development Kit (JDK 8 or higher)</li>
    <li>Apache Tomcat (or any Java Servlet container)</li>
    <li>PostgreSQL database</li>
    <li>IDE like Eclipse or IntelliJ IDEA for Java development</li>
</ul>

<h3>Steps</h3>

<ol>
    <li>Clone this repository:
        <pre><code>git clone https://github.com/RikGanguli/Online-Library-Management-System.git</code></pre>
    </li>
    <li>Set up PostgreSQL database:
        <ul>
            <li>Create a new database for the library system.</li>
            <li>Run the SQL scripts provided in the <code>sql/</code> folder to create the necessary tables and relationships.</li>
        </ul>
    </li>
    <li>Compile and deploy the web application:
        <ul>
            <li>Import the project into your Java IDE (Eclipse, IntelliJ, etc.).</li>
            <li>Build the project.</li>
            <li>Deploy the <code>.war</code> file or use your IDE's tools to deploy it on the Apache Tomcat server.</li>
        </ul>
    </li>
    <li>Start the server and access the application in your browser:
        <pre><code>http://localhost:8080/library-management-system</code></pre>
    </li>
</ol>

<h2 id="usage">Usage</h2>

<h3>Member Actions</h3>
<ul>
    <li><strong>Login</strong>: Members log in using their credentials to access the system.</li>
    <li><strong>Search for Documents</strong>: Search by title, author, publication year, etc.</li>
    <li><strong>Borrow Documents</strong>: Borrow available copies of documents.</li>
    <li><strong>Return Documents</strong>: Return borrowed documents before the due date to avoid fines.</li>
    <li><strong>Saved Searches</strong>: Save search queries for easy re-execution.</li>
</ul>

<h3>Librarian Actions</h3>
<ul>
    <li><strong>Manage Members</strong>: Add, edit, or remove member information.</li>
    <li><strong>Manage Documents</strong>: Add new documents, delete documents, or modify existing ones.</li>
    <li><strong>Overdue Tracking</strong>: Check which documents are overdue and notify members.</li>
</ul>

<h2>Credits</h2>
<p>Developed by Rik Ganguli Biswas</p>

