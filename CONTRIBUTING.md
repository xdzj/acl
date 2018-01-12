# How to contribute

Thank you for your interest in the Animation Compression Library! All contributions that follow our guidelines below and abide by our [code of conduct](CODE_OF_CONDUCT.md) are welcome. Together we can rid the video game world of slippery feet and jittery hands!

In this document you will find relevant reading material, what contributions we are looking for, and what we are *not* looking for.

Project contact email: zeno490@gmail.com

# Getting started

See the [readme](README.md) file for details on how to generate project solutions, build, and run the unit tests. Every pull request should run with continuous integration on every platform we support and the unit tests will also execute as well.

The project roadmap for the next few milestones is tracked with [GitHub issues](https://github.com/nfrechette/acl/issues). [Backlog issues](https://github.com/nfrechette/acl/milestone/4) are things I would like to get done eventually but that have not been prioritized yet.

Once you have identified an issue you would like to fix, comment on it first to make sure it is safe for you to claim it. Please only solve a single issue per pull request if at all possible. Unit tests are not absolutely required but they are welcome, especially for core functions.

Whether you create an issue or a pull request, I will do my best to comment or reply within 48 hours.

# Feature requests

Feature requests are welcome providing that they fit within the project scope. For smaller features, you are welcome to create an issue with as much relevant information as you can. If it makes sense, I will prioritize it or add it to the backlog, and if I feel it is beyond the scope of the project, I will tell you why and close the issue. For larger research topics to investigate, the best way to move forward is to reach out by email. Larger or exotic topics might best be worked on in their own research branch. Some might ultimately be included in the main branch if the results are attractive.

# Bug reports

The best way to report a bug is to provide necessary information for me to be able to reproduce it:

*  What environment you are using: OS, compiler, python version, etc.
*  What ACL version you are using.
*  How do you reproduce the issue and if applicable the compression and/or decompression settings used.
*  If at all possible include the offendind clip in the [ACL file format](./docs/the_acl_file_format.md) as it will allow a binary exact reproduction. If you would rather keep the clip private, you can forward it to me by email. I have no problem signing non-disclosure aggreements if required and your assets will be treated with the respect they deserve.

If you are observing accuracy issues and would like to report an issue about it, please make sure to double check what the measured error is reported as after the compression. An error threshold of **0.1mm** measured with a virtual vertex distance of **3.0cm** is in the vast majority of cases entirely acceptable for characters. As long as the virtual vertex distance on every bone reasonably approximates the visual mesh distance, ACL should be extremely accurate. In my experience, the overwhelming majority of gameplay animation accuracy issues comes from other systems.

# Contributions I am looking for

Several issues already have a [help wanted](https://github.com/nfrechette/acl/issues?q=is%3Aopen+is%3Aissue+label%3A%22help+wanted%22) label. Those tasks should be either reasonably simple or tasks that I do not think I will get the chance to get to very soon.

The topics where I am less savvy and would love help with are: anything to improve the continuous integration, adding unit tests, improving the documentation, adding example usage, and correcting or polishing my English as it is not my native language.

# Contributions I am *not* looking for

A lot of older compilers do not properly support **C++11** and there is no plan to support them. This also applies to platforms that are either not mainstream or that I cannot easily test with continuous integration. If you would like to support such an exotic environment, reach out by email first so we can discuss this.

This library's focus is solely on animation compression. There is no plan to include blending of animation poses or state machines to drive that process. Other middlewares and libraries already cover that field reasonably very well.

If you aren't sure, don't be afraid to reach out by email!
