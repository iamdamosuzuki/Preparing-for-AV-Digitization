# Preparing For AV Digitization
This workshop discusses the basics of Audiovisual Preservation, preparing for digitization audiovisual materials

## Description
This workshop will offer participants a general overview of the process of digitizing, migrating, and preserving your audiovisual collections. We will focus on media that are particularly at risk: analog video tapes (VHS, U-matic, Hi8), digital video tapes (MiniDV), and optical disc media (DVDs and CDs). You will learn the essential steps that are needed to digitize and migrate these media effectively, including: How to appropriately identify media for digitization, how to select preservation file formats, how to identify and use the necessary software and hardware for digitization and migration, and how to implement file management and digital preservation practices in order to ensure the successful preservation of your materials.


## Learning Objectives

After taking this course, participants will be able to:
  * Identify various at risk audiovisual media formats
  * Differentiate between analog and digital audiovisual media
  * Understand the difference between the terms “Digitize”, “Migrate”, and “Preserve” and recognize how these concepts are used in audiovisual preservation
  * Recognize the strengths and limitations of various digital media file formats
  * Confidently make determinations about which preservation file formats are best for their collections
  * Utilize open source software to analyze file-based media
  * Confidently store and maintain a collection of digitized media files

By the end of this course, participants should have a clear understanding of the fundamental concepts of digitizing, migrating, and preserving audiovisual media. Participants will also be prepared for the second course, which focuses on the hands-on processes of digitizing and migrating audiovisual media.

## Pre-Workshop Preparation

Before the workshop you'll need to install the following software:

  * [VLC](https://www.videolan.org/vlc/)
  * [MediaInfo](https://mediaarea.net/en/MediaInfo/Download)
  * [MediaConch](https://mediaarea.net/MediaConch)

Also, download this repository so you have access to the sample files the `MysterMedia` folder

## Exercise 1: File Use Cases

For this exercise we'll discuss a few different files. The instructor will poll the zoom to see which use case people think the files being discussed are best suited for.

  * File 1
    - MP4 Container
    - H.264 Encoding
    - Proprietary. This filetype is property of Apple
    - Highly compressed using lossy compression
    - Deinterlaced (video is optimized for viewing on a computer screen)
    - Audio Panned Center (audio is reorganized for a better listening experience)
    - 720x480
    - 100MB / hour (small enough to send on Google Drive)
    - <details>
      <summary>Click to see best use case</summary>
      Access
    </details>
  * File 2
    - MOV Container
    - ProRes Encoding
    - Proprietary This filetype is property of Apple
    - Mildly compressed using lossy compression
    - Deinterlaced (video is optimized for viewing on a computer screen)
    - Audio same as tape (audio has not been reorganized to easy viewing/listening)
    - 720x486
    - 30GB / hour (very large file, 30 hours would be one Terabyte)
    - <details>
      <summary>Click to see best use case</summary>
      Production
    </details>
  * File 3
    - MOV Container
    - V210 Encoding
    - Proprietary This filetype is property of Apple
    - Uncompressed
    - Interlaced (video is the same as on the tape)
    - Audio same as tape
    - 720x486
    - 100GB / hr (huge file size, 10 hours is a Terabyte)
    - <details>
      <summary>Click to see best use case</summary>
      Preservation
    </details>
  * File 4
    - MKV Container
    - FFV1 Encoding
    - Open Source (file specification is open and free to all)
    - Lossless compression
    - Interlaced (video is the same as on the tape)
    - Audio same as tape
    - 720x486
    - Internal Checksums (the file performs fixit checks on itself during playback and decoding)
    - 40GB / hr (large file size)
    - <details>
      <summary>Click to see best use case</summary>
      Preservation
    </details>
  * File 5
    - DV Container
    - DV Encoding
    - Proprietary
    - Mildly Lossy Compression
    - Interlaced
    - Audio same as tape
    - 720x480
    - 13GB / hr
    - <details>
      <summary>Click to see best use case</summary>
      Production
    </details>
  * File 5
    - MP4 Container
    - HEVC Encoding
    - Proprietary
    - Lossy Compression
    - Deinterlaced
    - Audio panned center
    - 1920x1080 (upscaled to HD)
    - 400MB / hr (small enough to send over the internet)
    - <details>
      <summary>Click to see best use case</summary>
      Access
    </details>

## Exercise 2: Preservation Formats

We've discussed how different types of media have different requirements for Preservation Formats. In this exercise we'll discuss different features that Preservation Formats can have and decide which media formats can benefit from these features.

1. Maintain Organization of Original
  * <details>
    <summary>Click to expand</summary>
    Analog Tape, Digital Tape, Optical Disc
    </details>
2. Lossless Compression
  * <details>
    <summary>Click to expand</summary>
    Analog Tape
    </details>
3. Complex Structure Capable of holding various Files
  * <details>
    <summary>Click to expand</summary>
    Optical Disc
    </details>
4. Uncompressed
  * <details>
    <summary>Click to expand</summary>
    Analog Tape
    </details>
5. Compatable With Common Playback Systems
  * <details>
    <summary>Click to expand</summary>
    None
    </details>
6. Open Source
  * <details>
    <summary>Click to expand</summary>
    Analog Tape, Digital Tape, Optical Disc
    </details>

## Exercise 3: Examining Files

For this exercise you're going to probe a bunch of mystery files and figure out what they are, and which might be a good candidate for a Preservation file. The files you'll need should have been downloaded with repository. They are in the `MysteryMedia` folder.

You can also right click the following links and press "Save Link As..." to save the files to your hard drive.

- [MysterFile01.mkv](https://github.com/iamdamosuzuki/Preparing-for-AV-Digitization/blob/main/MysteryMedia/MysteryFile01.mkv)
- [MysterFile02.mkv](https://github.com/iamdamosuzuki/Preparing-for-AV-Digitization/blob/main/MysteryMedia/MysteryFile02.mkv)
- [MysterFile03.mkv](https://github.com/iamdamosuzuki/Preparing-for-AV-Digitization/blob/main/MysteryMedia/MysteryFile03.mkv)
-[MysterFile04.mkv](https://github.com/iamdamosuzuki/Preparing-for-AV-Digitization/blob/main/MysteryMedia/MysteryFile04.mkv)

### Step 1: Play the files in VLC

To play files in VLC, open up VLC and drop the file you want to play into the window.

Note anything interesting that happens when you play the files

<details>
  <summary>When you're finished playing the files, click here to see some details you may have noticed</summary>
  - `MysterFile01` plays a standard definition video file
  - `MysterFile02` plays only audio
  - `MysterFile03` plays a high definition video file with no audio
  - `MysterFile04` plays a standard definition video file
</details>

### Step 2: Examine the files in MediaInfo

To play examine the files in MediaInfo, open up the program and drop the file you want to examine into the window.

You'll see the following information about the files:

  * General Information
  * Video Stream Information
  * Audio Stream Information

Do you see anything about the video information that matches up with what you saw when playing the files in VLC?

### Step 3: Examine the files in MediaConch

Now we'll use MediaConch to see if any of these files pass the policy named `Example MKV FFV1 Digitization Policy`.

Open MediaConch, click the `Checker` tab and drag all the files in. You should see them each populate as a row.

Next two where the program says `Apply a policy to all results`, select `Example MKV FFV1 Digitization Policy`.

Any files that are proper MKV FFV1 Preservation Files will show up in green, any that are not proper Preservation Files will show up in red. You can click the Eye icon in the red section to view what about the file caused it to fail the policy check.
