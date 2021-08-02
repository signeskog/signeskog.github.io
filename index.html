REMOVING ADAPTORS AND MAPPING GENOMIC FILES ON A WINDOWS

Preforming the first "clean up" steps of sequencing data is quite straight forward in a Linux environment. Although, not all have a linux computer on standby in teir office, nor
cloud space for big virtual machines. And still, there are some of us out there that have a background in wet lab biology, thrown into sequence analysis by an eager PI and with
limited experience in bash and console. 
Even if you have experience from some console coding before, like matlab and R, I was suprised by the lack of Windows supported options for the primary steps in sequence analysis,
removing the adaptors from your sequencing data. 

In this guide, I'll walk you through the process of using seqpac (which by the way is a great tool for the whole workflow of sequencing analysis) for the firsts steps of sequencing
data analysis, where we will go from fasta files downloaded from basespace (as my lab is using Illumina for seuqencing)

1.1 Install seqpac

Seqpac is an R based package, working in both Linux, Windows and Mac. In R, print and run

<devtools::install_github("Danis102/seqpac", upgrade="never", build_manual=TRUE, build_vignettes=TRUE)>

and then

<library(seqpac)>

to open up the package.

1.2 Perform adaptor trimming and quality control

First, we want to locate our files. If you, like me, are using the BaseSpace Downloader app from Illumina to download your fasta files, you can find the location of downloaded
files by opening the app. 

In seqpac, we now have two options. We can either use the make_counts command, to perform all primary steps in one go, or use make_trim

I'll start by showing you how make_counts work, but if you are only interested in make_trim, I'll walk you through that one too further down!

In seqpac, the major data analysis is performed on what's called a PAC (Pheno, Anno, Counts) object. With this first function make_counts, we create the count object
- transforming the fasta files into a object where we have samples as columns and each individual sequence as rows, as well as a number of how many times each sequence
is present in each sample (e.g how many "counts" that sequence have in a certain sample).
make_counts can take several details for you, like if and how strong you'd like a primary filter to be, what adaptors you were using and so on. I suggest you use
?make_counts if you are interested in learning more. 

But let's start with the easiest example. Let's say I have my fasta files in "D:/user/FASTA" and that I used Illumina adaptors in my laboratory preparation. Then, I can just
run this command:

<counts <- make_counts(input="D:/user/FASTA", trimming=TRUE)>

where I add the position on my computer in the input and telling the function that I want it to trim my fasta files with trimming=TRUE. That's it!

But what if I used a NEB-next adaptor, and for the sake of computer power wants to remove sequences that are not present in five individual samples 
(this can really help to speed up the coputational analysis, without removing sequences contributing to the analysis, see our preprint of seqpac for more information!)?
Then we could run make_counts, but with some modifications.

<counts <- make_counts(input="D:/user/FASTA", trimming=TRUE, parse="default_neb", evidence=c(experiment=5, sample=1), plot=TRUE)>

See that I added <plot=TRUE> too? This gives us a neat illustrative figure of how our samples behave, how the counts are distributed and how our evidence filters
affects the counts.

If you have a in-house adaptor, please check ?make_trim and ?make_counts examples to see how you can adjust for that!

Finally, it can sometimes be nice just to run the adaptor trimming alone. I then use the make_trim function, saving the fasta files after trimming into an output file.

<make_trim(input="D:/user/FASTA", output="D:/user/FASTA/output", adapt_3 = "AGATCGGAAGAGCACACGTCTGAACTCCAGTCACTA")
