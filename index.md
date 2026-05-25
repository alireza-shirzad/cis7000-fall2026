---
layout: default
title: "CIS 7000: Provably Secure Systems with Cryptography"
description: "University of Pennsylvania, Fall 2026"
---

# CIS 7000: Provably Secure Systems with Cryptography

<p class="lede">University of Pennsylvania &middot; Fall 2026</p>

## Basics

<ul class="basics">
  <li><strong>Instructors</strong> <a href="https://randomshuffle.github.io/">Anubhav Baweja</a>, <a href="https://pratyush.zip/">Pratyush Mishra</a>, <a href="https://alireza-shirzad.github.io/">Alireza Shirzad</a></li>
  <li><strong>Meetings</strong> Mondays and Wednesdays, 10:15&ndash;11:45 AM</li>
  <li><strong>Location</strong> TBD</li>
  <li><strong>Office hours</strong> By appointment</li>
  <li><strong>Ed Discussion</strong> TBD</li>
  <li><strong>Canvas</strong> TBD</li>
</ul>

## Description

This course explores how modern cryptography enables us to build real-world systems with rigorous, provable security and privacy guarantees. The course rests on two pillars &mdash; **applicability** and **provability**: we focus on constructions that address real-world problems while requiring that every system we study has mathematically provable security guarantees.

On the cryptographic side, we will explore advanced concepts including fully homomorphic encryption, zero-knowledge proofs, secure multi-party computation, private information retrieval, and oblivious RAM. We will then study real-world, practical systems built upon these ideas across a wide range of domains:

- **Machine learning** &mdash; private AI inference, privacy-preserving recommendation systems, and image/LLM watermarking.
- **Communication** &mdash; private and secure messaging.
- **Databases** &mdash; private and verifiable databases.
- **Cloud computing** &mdash; verifiable computation and secure aggregations.
- **Payments** &mdash; blockchains and related systems.
- **The Internet ecosystem** &mdash; Certificate Transparency and privacy-preserving middle-boxes.

Students will take an active role in presenting papers from top venues in cryptography, security, and systems, and exploring open problems alongside their peers. Students will also complete a research-oriented project that investigates an open question in provably secure systems &mdash; this can take the form of a new construction, security analysis, implementation, or empirical evaluation.

## Prerequisites

There are no formal prerequisites for this course, but students should be comfortable with **formal proofs** and **basic probability**. Prior exposure to cryptography is helpful but not required.

## Grading

| Component | Weight |
|---|---|
| Final project | 40% |
| Paper presentations | 30% |
| Peer project engagement | 30% |

## Schedule

The schedule below is tentative and will be updated throughout the semester. Topics, readings, and presenters will be filled in as the term progresses.

<p>
  <span class="tag tag-lecture">Lecture</span>
  <span class="tag tag-presentation">Presentation</span>
  <span class="tag tag-deadline">Deadline</span>
</p>

<table>
  <thead>
    <tr><th>Date</th><th>Topic</th><th>Required Reading</th><th>Optional Material</th></tr>
  </thead>
  <tbody>
    <tr class="module"><td colspan="4"><span class="module-num">MODULE 1</span>Introduction &amp; Foundations</td></tr>
    <tr>
      <td class="date"><span class="date-label">Wed Aug 26</span><span class="tag tag-lecture">Lecture</span></td>
      <td>
        <ul class="cell-list">
          <li>Introduction to the course (tools and logistics)</li>
          <li>Introduction to provable cryptography</li>
        </ul>
      </td>
      <td><a href="https://web.stanford.edu/class/ee384m/Handouts/HowtoReadPaper.pdf">How to Read a Paper</a></td>
      <td>
        <ul class="cell-list">
          <li><a href="https://www.youtube.com/watch?v=SPVWSG7-i_E">Caught in Between Theory and Practice</a></li>
          <li><a href="https://cseweb.ucsd.edu/~mihir/papers/isw-pops.pdf">Practice-Oriented Provable-Security</a></li>
          <li><a href="https://web.cs.ucdavis.edu/~rogaway/papers/cc.pdf">Practice-Oriented Provable Security and the Social Construction of Cryptography</a></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td class="date"><span class="date-label">Mon Aug 31</span><span class="tag tag-lecture">Lecture</span></td>
      <td>Introduction to provable cryptography (cont.)</td>
      <td><a href="https://www.amazon.com/Introduction-Cryptography-Chapman-Network-Security/dp/1466570261"><cite>Introduction to Modern Cryptography</cite></a>, Ch. 1</td>
      <td>
        <ul class="cell-list">
          <li><a href="https://joyofcryptography.com/"><cite>The Joy of Cryptography</cite></a>, &sect;4</li>
          <li><a href="https://www.karlin.mff.cuni.cz/~krajicek/ri5svetu.pdf">A Personal View of Average-Case Complexity</a></li>
        </ul>
      </td>
    </tr>
    <tr class="module"><td colspan="4"><span class="module-num">MODULE 2</span>Private Information Retrieval (PIR)</td></tr>
    <tr>
      <td class="date"><span class="date-label">Wed Sep 2</span><span class="tag tag-lecture">Lecture</span></td>
      <td>Motivation and construction</td>
      <td><a href="https://eprint.iacr.org/2022/949">One Server for the Price of Two: Simple and Fast Single-Server Private Information Retrieval</a></td>
      <td>&mdash;</td>
    </tr>
    <tr class="holiday"><td class="date"><span class="date-label">Mon Sep 7</span></td><td>No class &mdash; Labor Day</td><td>&mdash;</td><td>&mdash;</td></tr>
    <tr>
      <td class="date"><span class="date-label">Wed Sep 9</span><span class="tag tag-lecture">Lecture</span><span class="tag tag-presentation">Presentation</span></td>
      <td>Private browsing and recommendation systems: Tiptoe, Nudge</td>
      <td><a href="https://eprint.iacr.org/2023/1438">Private Web Search with Tiptoe</a></td>
      <td><a href="https://www.usenix.org/conference/usenixsecurity26/presentation/henzinger">Nudge: A Private Recommendations Engine</a></td>
    </tr>
    <tr>
      <td class="date"><span class="date-label">Mon Sep 14</span><span class="tag tag-lecture">Lecture</span><span class="tag tag-presentation">Presentation</span></td>
      <td>Private messaging and metadata-hiding communication: Pung, Addra, Express, PIR-Tor, PerfOMR</td>
      <td><a href="https://www.usenix.org/system/files/conference/osdi16/osdi16-angel.pdf">Unobservable Communication over Fully Untrusted Infrastructure</a></td>
      <td>&mdash;</td>
    </tr>
    <tr class="module"><td colspan="4"><span class="module-num">MODULE 3</span>Secure Messaging</td></tr>
    <tr>
      <td class="date"><span class="date-label">Wed Sep 16</span><span class="tag tag-lecture">Lecture</span></td>
      <td>Mixnets</td>
      <td>&mdash;</td>
      <td>&mdash;</td>
    </tr>
    <tr>
      <td class="date"><span class="date-label">Mon Sep 21</span><span class="tag tag-lecture">Lecture</span><span class="tag tag-presentation">Presentation</span></td>
      <td>Onion routing</td>
      <td><a href="http://dud.inf.tu-dresden.de/literatur/Anon_Terminology_v0.31.pdf">Anonymity Terminology</a> (Pfitzmann &amp; Hansen)</td>
      <td>
        <ul class="cell-list">
          <li><a href="https://svn.torproject.org/svn/projects/design-paper/tor-design.pdf">Tor: The Second-Generation Onion Router</a></li>
          <li><a href="https://davidlazar.org/papers/vuvuzela.pdf">Vuvuzela: Scalable Private Messaging Resistant to Traffic Analysis</a></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td class="date"><span class="date-label">Mon Sep 28</span><span class="tag tag-lecture">Lecture</span><span class="tag tag-presentation">Presentation</span></td>
      <td>Metadata-private messaging via DPF and FSS</td>
      <td><a href="https://eprint.iacr.org/2025/687">Myco: Unlocking Polylogarithmic Accesses in Metadata-Private Messaging</a></td>
      <td>
        <ul class="cell-list">
          <li><a href="https://www.usenix.org/system/files/conference/osdi16/osdi16-angel.pdf">Unobservable Communication over Fully Untrusted Infrastructure</a></li>
          <li>Distributed Point Functions</li>
          <li>Function Secret Sharing</li>
          <li>Riposte: An Anonymous Messaging System Handling Millions of Users</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td class="date"><span class="date-label">Wed Sep 30</span><span class="tag tag-lecture">Lecture</span></td>
      <td>Message franking</td>
      <td>&mdash;</td>
      <td>&mdash;</td>
    </tr>
    <tr class="module"><td colspan="4"><span class="module-num">MODULE 4</span>Transparency Logs, Bulletin Boards and Blockchain</td></tr>
    <tr>
      <td class="date"><span class="date-label">Mon Oct 5</span><span class="tag tag-lecture">Lecture</span><span class="tag tag-presentation">Presentation</span></td>
      <td>
        <ul class="cell-list">
          <li>Polynomial commitments</li>
          <li>Key &amp; certificate transparency</li>
        </ul>
      </td>
      <td><a href="https://eprint.iacr.org/2025/1580">IronDict: Transparent Dictionaries from Polynomial Commitments</a></td>
      <td>
        <ul class="cell-list">
          <li><a href="https://engineering.fb.com/2023/04/13/security/whatsapp-key-transparency/">Deploying Key Transparency at WhatsApp</a></li>
          <li><a href="https://certificate.transparency.dev/howctworks/">How CT Fits into the Wider Web PKI Ecosystem</a></li>
          <li><a href="https://spawn-queue.acm.org/doi/pdf/10.1145/2668152.2668154">Certificate Transparency: Public, Verifiable, Append-Only Logs</a></li>
          <li><a href="https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9592820">Certificate Transparency in Google Chrome: Past, Present, and Future</a></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td class="date"><span class="date-label">Wed Oct 7</span><span class="tag tag-lecture">Lecture</span><span class="tag tag-presentation">Presentation</span></td>
      <td>
        <ul class="cell-list">
          <li>Bitcoin</li>
          <li>Ethereum</li>
        </ul>
      </td>
      <td><a href="https://bitcoin.org/bitcoin.pdf">Bitcoin: A Peer-to-Peer Electronic Cash System</a></td>
      <td>&mdash;</td>
    </tr>
    <tr>
      <td class="date"><span class="date-label">Mon Oct 12</span><span class="tag tag-lecture">Lecture</span><span class="tag tag-presentation">Presentation</span></td>
      <td>
        <ul class="cell-list">
          <li>Zero-knowledge proofs</li>
          <li>Private blockchains</li>
        </ul>
      </td>
      <td><a href="https://eprint.iacr.org/2014/349.pdf">Zerocash: Decentralized Anonymous Payments from Bitcoin</a></td>
      <td><a href="https://eprint.iacr.org/2018/962">Zexe: Enabling Decentralized Private Computation</a></td>
    </tr>
    <tr class="module"><td colspan="4"><span class="module-num">MODULE 5</span>Proof Systems</td></tr>
    <tr>
      <td class="date"><span class="date-label">Wed Oct 14</span><span class="tag tag-lecture">Lecture</span><span class="tag tag-presentation">Presentation</span></td>
      <td>
        <ul class="cell-list">
          <li>R1CS</li>
          <li>Groth16</li>
        </ul>
      </td>
      <td><a href="https://eprint.iacr.org/2016/260">On the Size of Pairing-Based Non-Interactive Arguments</a></td>
      <td>&mdash;</td>
    </tr>
    <tr>
      <td class="date"><span class="date-label">Mon Oct 19</span><span class="tag tag-lecture">Lecture</span><span class="tag tag-presentation">Presentation</span></td>
      <td>zk-VMs</td>
      <td><a href="https://eprint.iacr.org/2013/507">SNARKs for C: Verifying Program Executions Succinctly and in Zero Knowledge</a></td>
      <td><a href="https://github.com/rkdud007/awesome-zkvm">awesome-zkVM</a></td>
    </tr>
    <tr>
      <td class="date"><span class="date-label">Wed Oct 21</span><span class="tag tag-lecture">Lecture</span><span class="tag tag-presentation">Presentation</span></td>
      <td>zk-credentials, zk-TLS</td>
      <td>zk-creds: Flexible Anonymous Credentials from zkSNARKs and Existing Identity Infrastructure</td>
      <td>&mdash;</td>
    </tr>
    <tr>
      <td class="date"><span class="date-label">Mon Oct 26</span><span class="tag tag-lecture">Lecture</span><span class="tag tag-presentation">Presentation</span></td>
      <td>VerITAS</td>
      <td><a href="https://eprint.iacr.org/2024/1066">VerITAS: Verifying Image Transformations at Scale</a></td>
      <td>&mdash;</td>
    </tr>
    <tr class="module"><td colspan="4"><span class="module-num">MODULE 6</span>Watermarking and Model Stealing</td></tr>
    <tr>
      <td class="date"><span class="date-label">Wed Oct 28</span><span class="tag tag-lecture">Lecture</span><span class="tag tag-presentation">Presentation</span></td>
      <td>Pseudorandom codes</td>
      <td><a href="https://arxiv.org/pdf/2306.09194">Undetectable Watermarks for Language Models</a></td>
      <td><a href="https://arxiv.org/abs/2411.18479">arXiv:2411.18479</a></td>
    </tr>
    <tr>
      <td class="date"><span class="date-label">Mon Nov 2</span><span class="tag tag-lecture">Lecture</span><span class="tag tag-presentation">Presentation</span></td>
      <td>Model stealing</td>
      <td><a href="https://arxiv.org/pdf/2410.05750">Polynomial Time Cryptanalytic Extraction of Deep Neural Networks in the Hard-Label Setting</a></td>
      <td>&mdash;</td>
    </tr>
    <tr><td class="date"><span class="date-label">Wed Nov 4</span><span class="tag tag-presentation">Presentation</span></td><td>TBD</td><td>&mdash;</td><td>&mdash;</td></tr>
    <tr><td class="date"><span class="date-label">Fri Nov 6</span><span class="tag tag-deadline">Deadline</span></td><td>Project proposal due</td><td>&mdash;</td><td>&mdash;</td></tr>
    <tr class="module"><td colspan="4"><span class="module-num">MODULE 7</span>Fully Homomorphic Encryption (FHE)</td></tr>
    <tr>
      <td class="date"><span class="date-label">Mon Nov 9</span><span class="tag tag-lecture">Lecture</span></td>
      <td>
        <ul class="cell-list">
          <li>Linear homomorphism to full homomorphism</li>
          <li>Bootstrapping</li>
        </ul>
      </td>
      <td><a href="https://crypto.stanford.edu/craig/easy-fhe.pdf">Computing Arbitrary Functions of Encrypted Data</a></td>
      <td>&mdash;</td>
    </tr>
    <tr>
      <td class="date"><span class="date-label">Wed Nov 11</span><span class="tag tag-lecture">Lecture</span><span class="tag tag-presentation">Presentation</span></td>
      <td>Private AI inference (part 1)</td>
      <td><a href="https://icml.cc/virtual/2025/poster/45395">EncryptedLLM: Privacy-Preserving Large Language Model Inference via GPU-Accelerated Fully Homomorphic Encryption</a></td>
      <td><a href="https://docs.zama.org/concrete-ml">Concrete ML</a></td>
    </tr>
    <tr>
      <td class="date"><span class="date-label">Mon Nov 16</span><span class="tag tag-lecture">Lecture</span><span class="tag tag-presentation">Presentation</span></td>
      <td>Private AI inference (part 2)</td>
      <td><a href="https://arxiv.org/abs/2410.09457">Power-Softmax: Towards Secure LLM Inference over Encrypted Data</a></td>
      <td><a href="https://arxiv.org/abs/2501.01672">Practical Secure Inference Algorithm for Fine-Tuned Large Language Model Based on Fully Homomorphic Encryption</a></td>
    </tr>
    <tr class="module"><td colspan="4"><span class="module-num">MODULE 8</span>Oblivious RAM (ORAM)</td></tr>
    <tr>
      <td class="date"><span class="date-label">Wed Nov 18</span><span class="tag tag-lecture">Lecture</span></td>
      <td>
        <ul class="cell-list">
          <li>Motivation</li>
          <li>Definition</li>
          <li>Constructions</li>
        </ul>
      </td>
      <td>&mdash;</td>
      <td>&mdash;</td>
    </tr>
    <tr>
      <td class="date"><span class="date-label">Mon Nov 23</span><span class="tag tag-lecture">Lecture</span><span class="tag tag-presentation">Presentation</span></td>
      <td>Zoom Contact Discovery / Encrypted databases and analytics: Opaque, ObliDB</td>
      <td>&mdash;</td>
      <td>&mdash;</td>
    </tr>
    <tr class="holiday"><td class="date"><span class="date-label">Wed Nov 25</span></td><td>No class &mdash; Thanksgiving</td><td>&mdash;</td><td>&mdash;</td></tr>
    <tr class="module"><td colspan="4"><span class="module-num">MODULE 9</span>Final Projects</td></tr>
    <tr><td class="date"><span class="date-label">Mon Nov 30</span></td><td>Final presentations</td><td>&mdash;</td><td>&mdash;</td></tr>
    <tr><td class="date"><span class="date-label">Wed Dec 2</span></td><td>Final presentations</td><td>&mdash;</td><td>&mdash;</td></tr>
    <tr><td class="date"><span class="date-label">Mon Dec 7</span></td><td>Final presentations</td><td>&mdash;</td><td>&mdash;</td></tr>
    <tr><td class="date"><span class="date-label">Wed Dec 9</span></td><td>Final presentations</td><td>&mdash;</td><td>&mdash;</td></tr>
    <tr><td class="date"><span class="date-label">Mon Dec 14</span><span class="tag tag-deadline">Deadline</span></td><td>Final reports due</td><td>&mdash;</td><td>&mdash;</td></tr>
  </tbody>
</table>

## Course components

### Reading responses

Most discussion-format classes are paired with a paper. Students submit short-answer responses to a few prompts about the paper **before class**. These are graded for completion and used to seed in-class discussion.

### Paper presentations

Sessions in the schedule are tagged by format:

- <span class="tag tag-lecture">Lecture</span> &mdash; a full lecture led by the instructors. No student presentation that day.
- <span class="tag tag-presentation">Presentation</span> &mdash; a student leads the discussion of the day's paper.
- <span class="tag tag-lecture">Lecture</span> <span class="tag tag-presentation">Presentation</span> &mdash; the instructors lecture on foundational material and a student presents the day's paper in the same session.

Every student presents **at least once**. Depending on enrollment, each student may end up presenting **twice or more** &mdash; we will distribute presentation slots based on class size.

A good presentation:

- Motivates the problem the paper addresses.
- Describes the paper's main contributions and the techniques used.
- Identifies the security model and proof strategy.
- Highlights limitations and open questions for class discussion.

Papers are drawn from suggested venues including CRYPTO, EUROCRYPT, S&amp;P, CCS, USENIX Security, NDSS, OSDI, SOSP, and NSDI.

### Peer project engagement

Project work benefits from a community of reviewers. Every student is expected to engage substantively with their classmates' projects, not just their own. Concretely, this means:

- **Attend every final presentation session** during the last weeks of the semester.
- **Read and review peers' project proposals and drafts**, and provide written feedback when asked.
- **Brainstorm and ask questions** during classmates' presentations &mdash; help them sharpen ideas, surface gaps, and identify open directions.

Graded on the depth, consistency, and constructiveness of your contributions to others' projects.

### Final project

The final project is a research-oriented investigation of an open question in provably secure systems. Acceptable directions include:

- A **new construction** of a cryptographic primitive or system.
- A **security analysis** of an existing scheme or deployed system.
- An **implementation** and benchmarking of a known construction.
- An **empirical evaluation** comparing approaches in a particular application domain.

Projects may be done in teams of **1&ndash;2 students**. Deliverables:

- **Proposal** (~2 pages) &mdash; problem statement, related work, plan, and evaluation criteria.
- **Presentation** &mdash; ~15-minute talk in the final weeks of the semester.
- **Report** (~8&ndash;12 pages) &mdash; written in the style of a workshop submission.

## Policies

**Collaboration.** Discussion of course material with classmates is encouraged. All written work submitted under your name must be your own. Cite all sources, including conversations with peers and any AI tools used.

**Academic integrity.** Standard [Penn Code of Academic Integrity](https://catalog.upenn.edu/pennbook/code-of-academic-integrity/) applies.

**Accommodations.** Students requesting accommodations should contact [Weingarten Center](https://weingartencenter.universitylife.upenn.edu/) at the start of the semester.
