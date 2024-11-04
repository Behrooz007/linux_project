<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Linux Project README</title>
</head>
<body>
    <h1>Linux Project: Directory Management, Archiving, and Compression</h1>

    <h2>Project Overview</h2>
    <p>This project demonstrates basic Linux command-line operations to organize, archive, compress, and extract files. Through this project, you will become familiar with directory structure management and compression techniques using tools like <code>tar</code> and <code>gzip</code>.</p>

    <h3>Project Structure and Setup</h3>
    <ol>
        <li><strong>Create the Main Project Directory:</strong>
            <pre><code>mkdir ArchiveProject
cd ArchiveProject</code></pre>
        </li>
        <li><strong>Create Subdirectories:</strong>
            <pre><code>mkdir dir1 dir2 dir3</code></pre>
        </li>
        <li><strong>Add Sample Files to Each Directory:</strong>
            <pre><code>echo "This is file1 in dir1" > dir1/file1.txt
echo "This is file2 in dir2" > dir2/file2.txt
echo "This is file3 in dir3" > dir3/file3.txt</code></pre>
            <p>Directory structure after setup:</p>
            <pre><code>ArchiveProject/
├── dir1/
│   └── file1.txt
├── dir2/
│   └── file2.txt
└── dir3/
    └── file3.txt</code></pre>
        </li>
    </ol>

    <h3>Archiving and Compressing the Directories</h3>
    <ol start="4">
        <li><strong>Archive the Directories:</strong>
            <pre><code>cd ..
tar -cvf project_archive.tar ArchiveProject</code></pre>
        </li>
        <li><strong>Compress the Archive:</strong>
            <pre><code>gzip project_archive.tar</code></pre>
            <p>Resulting in <code>project_archive.tar.gz</code>.</p>
        </li>
    </ol>

    <h3>Extraction Process</h3>
    <ol start="6">
        <li><strong>Set Up for Extraction:</strong>
            <pre><code>mkdir ExtractedArchive
mv project_archive.tar.gz ExtractedArchive/
cd ExtractedArchive</code></pre>
        </li>
        <li><strong>Decompress and Extract:</strong>
            <pre><code>tar -xzvf project_archive.tar.gz</code></pre>
            <p>This will restore the <code>ArchiveProject</code> directory structure within <code>ExtractedArchive</code>.</p>
        </li>
        <li><strong>Verify the Extraction:</strong>
            <pre><code>ls -R ArchiveProject</code></pre>
        </li>
    </ol>

    <h2>Summary of Commands</h2>
    <ul>
        <li><strong>Directory and File Creation:</strong> <code>mkdir</code>, <code>echo</code></li>
        <li><strong>Archiving:</strong> <code>tar -cvf</code></li>
        <li><strong>Compression:</strong> <code>gzip</code></li>
        <li><strong>Extraction and Decompression:</strong> <code>tar -xzvf</code></li>
    </ul>

    <h2>Learning Outcomes</h2>
    <p>By completing this project, you will:</p>
    <ul>
        <li>Learn Linux directory and file management commands.</li>
        <li>Gain proficiency with <code>tar</code> for archiving.</li>
        <li>Understand compression with <code>gzip</code>.</li>
        <li>Practice decompression and extraction.</li>
        <li>Improve command-line efficiency for file management.</li>
        <li>Develop foundational skills in backup and storage management.</li>
    </ul>

    <h2>Author</h2>
    <p><strong>Student Name:</strong> Behrooz Rashidi</p>
    <p><strong>UID:</strong> 24MCA20423</p>
    <p><strong>Branch:</strong> MCA</p>
</body>
</html>
