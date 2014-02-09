samtools
========

This is a modified verion of samtools for a project needing a specific text/html view of a bam alignment.
Modifications are under 'standalone' branch, tagged 'my-html-tview-1'

Mods:

- Specify -d h to trigger HTML output
- Specify -p chr:pos to specify coordinate to center window on
- Bases will be colored by base quality
- Center base will be underlined in reads
- Center base will be title of page and body
- Legend for codes at bottom of page
- View of 120-130 bases across page

Usage:

    samtools tview -d h -p pos-to-center-on in.bam ref.fasta
eg:

    samtools tview -d h -p chr12:25398284  my.bam hg19.fasta > my.html


See also http://github.com/samtools/

