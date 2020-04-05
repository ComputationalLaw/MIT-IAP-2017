<span class="c28 c32">CV19 Contact Tracing Privacy Principles</span>

<span class="c14"></span>

<span class="c14">The Law.MIT.edu research team is actively collecting and curating privacy principles for contact tracing applications and services that leverage personal individual location and proximity data.  We intend to publish key developments in this space on an ongoing basis through the MIT Computational Law Report Special Release on CV19 Legal Frameworks.</span>

<span class="c14"></span>

<span class="c0">[Draft Contact Tracing Privacy Principles](#h.k0nje0ariiwi)</span>

<span class="c0">[1\. Summary](#h.ysn5e3sonydq)</span>

<span class="c0">[2\. Technology should follow the principles of Privacy by Design](#h.edj5m221nyg7)</span>

<span class="c0">[3\. Data should be protected in accordance with Fair Information Practice Principles (FIPPs)](#h.6g06ff6uv7c6)</span>

<span class="c0">[Notice/Awareness](#h.jwnvwof2htkm)</span>

<span class="c0">[Choice/Consent](#h.c8zceb4xajsh)</span>

<span class="c0">[Implementation guidance:](#h.uth9m5m6xghq)</span>

<span class="c0">[Access/Participation](#h.o21mpm3ysyuo)</span>

<span class="c0">[Integrity/Security](#h.xeor3bak2vpc)</span>

<span class="c0">[Enforcement/Redress](#h.fvzl0kc7ifg4)</span>

<span class="c0">[4\. Potential Application of these Principles to Location MIT Private Kit: Safe Paths Open Source](#h.1foq4fkt906a)</span>

<span class="c0">[Contact Tracing Bill of Rights](#h.f0mutkbx6xft)</span>

<span class="c0">[1\. Users must be able to install and use a contact tracing app without having to divulge any personal information to anyone.](#h.ygz1xggjp2wt)</span>

<span class="c0">[2\. Contact tracing apps must not disclose any information during normal operation that can be used by third parties to track a user’s interactions or locations.](#h.ayoycus9hst)</span>

<span class="c0">[3\. All information disclosed by users through a contact-tracing app must be completely opt-in, with clear informed consent both as to the nature of what they’re disclosing and the likely impacts of doing so.](#h.gd2so8r7hph4)</span>

<span class="c0">[4\. When users choose to altruistically share information, that information must remain completely anonymous: no information may be required other than that which is essential for alerting others to potential exposure.](#h.sx34lqgi3nav)</span>

<span class="c0">[5\. If apps collect any information, such as location histories, that is not essential for alerting others who may be exposed, users must not be expected or coerced to share that information by default. If a contact tracing app allows for the sharing of any location history, symptom reports, demographic information, or similar with public health officials or similar, such sharing must be completely anonymous, voluntary, and opt-in, and based on clear and easy to understand informed consent.](#h.vhsyard90fi)</span>

<span class="c0">[Evaluating COVID-19 contact tracing apps? Here are 8 privacy questions we think you should ask.](#h.4m50sknizfqi)</span>

<span class="c0">[Contact tracing – Setup](#h.pptbpoc3pm3o)</span>

<span class="c0">[Toy protocol 1 (using location):](#h.stqdsj1o5to8)</span>

<span class="c0">[Toy protocol 2 (using Bluetooth):](#h.qp8f4d3t348u)</span>

<span class="c0">[Toy protocol 3 (using Bluetooth):](#h.jyjsujpvj42g)</span>

<span class="c0">[The questions](#h.o1aorpmkhufd)</span>

<span class="c0">[1\. How do you limit the personal data gathered by the authority?](#h.6z2vw7pb27bs)</span>

<span class="c0">[2\. How do you protect the anonymity of every user?](#h.uf8wju5w8tne)</span>

<span class="c0">[3\. Does your system reveal to the authority the identity of users who are at risk?](#h.r7tkm8npp89n)</span>

<span class="c0">[4\. Could your system be used by users to learn who is infected or at risk, even in their social circle?](#h.p7awcuouxmto)</span>

<span class="c0">[5\. Does your system allow users to learn any personal information about other users?](#h.me1t82c85wyz)</span>

<span class="c0">[6\. Could external parties exploit your system to track users or infer whether they are infected?](#h.a2rvhg79trut)</span>

<span class="c0">[7\. Do you put in place additional measures to protect the personal data of infected and at risk users?](#h.8ypgh5rvy8ym)</span>

<span class="c0">[8\. How can we verify that the system does what it says?](#h.rysfytiuzn50)</span>

<span class="c14"></span>

# <span class="c13">Draft Contact Tracing Privacy Principles</span>

## <span class="c6">1\. Summary</span>

*   <span class="c41">Each of us is the primary owner of our personal data.  </span><span class="c14">Services that we each use may have additional limited rights and responsibilities to our personal data, based on specified terms and conditions appropriate to the service.  A doctor, for example, has the right to maintain patient data and the responsibility to preserve it and only share it with patient consent.</span>
*   <span class="c41">Health, education, location, and contact tracing data is personal data.</span><span class="c14">  No service provider or government agency should be able to use that data without user consent.</span>

<span class="c39 c28"></span>

## <span>2\. Technology should follow the principles of</span> <span class="c31">[Privacy by Design](https://www.google.com/url?q=https://en.wikipedia.org/wiki/Privacy_by_design&sa=D&ust=1586111888569000)</span>

*   <span class="c14">Proactive not reactive; preventive, not remedial</span>
*   <span class="c14">Privacy as the default</span>
*   <span class="c14">Privacy embedded in the design</span>
*   <span class="c14">Full functionality – positive-sum, not zero-sum</span>
*   <span class="c14">End-to-end security – full lifecycle protection</span>
*   <span class="c14">Visibility and transparency – keep it open</span>
*   <span class="c14">Respect for user privacy – keep it user-centric</span>

<span class="c39 c28"></span>

## <span>3\. Data should be protected in accordance with</span> <span class="c31">[Fair Information Practice Principles (FIPPs)](https://www.google.com/url?q=https://en.wikipedia.org/wiki/FTC_fair_information_practice&sa=D&ust=1586111888570000)</span>

*   ### <span class="c41">Notice/Awareness</span>

<span class="c14">Consumers should be given notice of an entity's information practices before any personal information is collected from them.[10] This requires that companies explicitly notify some or all of the following:</span>

*   <span class="c14">identification of the entity collecting the data;</span>
*   <span class="c14">identification of the uses to which the data will be put;</span>
*   <span class="c14">identification of any potential recipients of the data;</span>
*   <span class="c14">the nature of the data collected and the means by which it is collected;</span>
*   <span class="c14">whether the provision of the requested data is voluntary or required;</span>
*   <span class="c14">the steps taken by the data collector to ensure the confidentiality, integrity, and quality of the data.</span>

<span class="c14"></span>

*   ### <span class="c19">Choice/Consent</span>

<span class="c14">Choice and consent in an on-line information-gathering sense means giving consumers options to control how their data is used. Specifically, choice relates to secondary uses of information beyond the immediate needs of the information collector to complete the consumer's transaction. The two typical types of choice models are 'opt-in' or 'opt-out.'</span>

1.  <span class="c14">The 'opt-in' method requires that consumers affirmatively give permission for their information to be used for other purposes. Without the consumer taking these affirmative steps in an 'opt-in' system, the information gatherer assumes that it cannot use the information for any other purpose.</span>
2.  <span class="c14">The 'opt-out' method requires consumers to affirmatively decline permission for other uses. Without the consumer taking these affirmative steps in an 'opt-out' system, the information gatherer assumes that it can use the consumer's information for other purposes.</span>

<span class="c14">Each of these systems can be designed to allow an individual consumer to tailor the information gatherer's use of the information to fit their preferences by checking boxes to grant or deny permission for specific purposes rather than using a simple "all or nothing" method.</span>

<span class="c14"></span>

*   #### <span class="c42">Implementation guidance:</span>

*   <span class="c27 c28">It is recommended that the opt-in consent option is implemented as that will comply with a good number of data protection laws globally</span>
*   <span class="c27 c28">Template consent language like the below should be considered:</span>

<span class="c30">“I consent to (</span><span class="c30 c45">Add Controller Name OR App Name if whitelabelled to the Controller</span><span class="c27 c28">) processing my:</span>

<span class="c27 c28">(Add unticked checkbox OR toggle off) Location data</span>

<span class="c30">(Add unticked checkbox OR toggle off) Health data for the purpose of COVID 19 contact tracing in accordance with the (</span><span class="c30 c43">Add link to the Controller Privacy Notice</span><span class="c27 c28">).”</span>

*   <span class="c27 c28">There are alternative ways to present substantially similar text in the UX. E.g. splitting the screens and adding a “continue” button. Then the language will be adapted to “By clicking continue..”</span>

<span class="c27 c28"></span>

*   ### <span class="c19">Access/Participation</span>

<span class="c14">Access includes not only a consumer's ability to view the data collected but also to verify and contest its accuracy. This access must be inexpensive and timely in order to be useful to the consumer.</span>

<span class="c14"></span>

*   ### <span class="c19">Integrity/Security</span>

<span class="c14"> Information collectors should ensure that the data they collect is accurate and secure. They can improve the integrity of data by cross-referencing it with only reputable databases and by providing access for the consumer to verify it. Information collectors can keep their data secure by protecting against both internal and external security threats. They can limit access within their company to only necessary employees to protect against internal threats, and they can use encryption and other computer-based security systems to stop outside threats.</span>

<span class="c14"></span>

*   ### <span class="c19">Enforcement/Redress</span>

<span class="c14"> In order to ensure that companies follow the Fair Information Practice Principles, there must be enforcement measures. The FTC identified three types of enforcement measures: self-regulation by the information collectors or an appointed regulatory body; private remedies that give civil causes of action for individuals whose information has been misused to sue violators; and government enforcement that can include civil and criminal penalties levied by the government.</span>

<span class="c28 c39"></span>

## <span class="c6">4\. Potential Application of these Principles to Location MIT Private Kit: Safe Paths Open Source</span>

*   <span class="c14">Possible contacts determined privately on a user’s own device using open source code and cryptographic algorithms</span>
*   <span class="c14">Data never leave the user’s device (100% local), unless they become ill and opt to release it to a health official</span>
*   <span class="c14">Trusted health officials remove all diagnosed patient personally identifiable information – only releasing the redacted location trail</span>
*   <span>O</span><span class="c14 c10">nly release the redacted, disconnected, and aggregated space-time points</span>
*   <span class="c10">Space-time points</span> <span class="c10 c40">will be deleted after they are no longer actively needed, estimated at between 21 and 28 days.</span>

<span class="c14"></span>

* * *

<span class="c14"></span>

# <span class="c13">Contact Tracing Bill of Rights</span>

*   <span class="c14">Developed by: CoEpi and CovidWatch Source:</span>
*   <span class="c31">[https://github.com/Co-Epi/CEN/blob/main/ContactTracingBillOfRights.md](https://www.google.com/url?q=https://github.com/Co-Epi/CEN/blob/main/ContactTracingBillOfRights.md&sa=D&ust=1586111888575000)</span><span class="c14"> </span>

<span class="c14"></span>

## <span>1\.</span> <span class="c9">Users must be able to install and use a contact tracing app without having to divulge any personal information to anyone.</span>

<span class="c17 c25"></span>

## <span class="c6">2\. Contact tracing apps must not disclose any information during normal operation that can be used by third parties to track a user’s interactions or locations.</span>

<span class="c17 c25"></span>

## <span class="c6">3\. All information disclosed by users through a contact-tracing app must be completely opt-in, with clear informed consent both as to the nature of what they’re disclosing and the likely impacts of doing so.</span>

<span class="c17 c25"></span>

## <span class="c6">4\. When users choose to altruistically share information, that information must remain completely anonymous: no information may be required other than that which is essential for alerting others to potential exposure.</span>

<span class="c17 c25"></span>

### <span class="c19">5\. If apps collect any information, such as location histories, that is not essential for alerting others who may be exposed, users must not be expected or coerced to share that information by default. If a contact tracing app allows for the sharing of any location history, symptom reports, demographic information, or similar with public health officials or similar, such sharing must be completely anonymous, voluntary, and opt-in, and based on clear and easy to understand informed consent.</span>

<span class="c14"></span>

<span class="c14"></span>

* * *

<span class="c14"></span>

<span class="c14"></span>

# <span class="c13">Evaluating COVID-19 contact tracing apps? Here are 8 privacy questions we think you should ask.</span>

*   <span class="c14">Developed by: Yves-Alexandre de Montjoye, Florimond Houssiau, Andrea Gadotti and Florent Guepin</span>
*   <span class="c14">As collected on April 2, 2020</span>

*   <span class="c31">[https://cpg.doc.ic.ac.uk/blog/evaluating-contact-tracing-apps-here-are-8-privacy-questions-we-think-you-should-ask](https://www.google.com/url?q=https://cpg.doc.ic.ac.uk/blog/evaluating-contact-tracing-apps-here-are-8-privacy-questions-we-think-you-should-ask&sa=D&ust=1586111888578000)</span><span class="c14"> </span>

<span class="c17 c10 c47"></span>

<span class="c7">As strong measures are being put in place to slow down the spread of COVID-19, many are looking at how technology and data could help. With</span> <span class="c11 c10">[many](https://www.google.com/url?q=https://plus.lesoir.be/286535/article/2020-03-12/coronavirus-le-cabinet-de-block-dit-oui-lutilisation-des-donnees-telecoms&sa=D&ust=1586111888578000)</span><span class="c7"> </span><span class="c11 c10">[countries](https://www.google.com/url?q=https://www.theguardian.com/world/2020/mar/19/plan-phone-location-data-assist-uk-coronavirus-effort&sa=D&ust=1586111888579000)</span><span class="c7"> </span><span class="c11 c10">[using mobile phone](https://www.google.com/url?q=https://edition.cnn.com/2020/03/18/tech/us-government-location-data-coronavirus/index.html&sa=D&ust=1586111888579000)</span><span class="c7"> </span><span class="c11 c10">[location](https://www.google.com/url?q=https://www.politico.eu/article/european-commission-mobile-phone-data-thierry-breton-coronavirus-covid19/&sa=D&ust=1586111888579000)</span><span class="c7"> </span><span class="c11 c10">[data](https://www.google.com/url?q=https://www.timesofisrael.com/health-ministry-begins-controversial-tracking-of-coronavirus-patients&sa=D&ust=1586111888579000)</span><span class="c17 c7"> to analyze the effectiveness of social distancing measures and help predict the potential geographic spread of the disease, the focus has now shifted to whether mobile phones could also help warn users if they have been exposed to an infected person.</span>

<span class="c7">Contact tracing apps are being developed in the</span> <span class="c11 c10">[UK](https://www.google.com/url?q=https://news.sky.com/story/coronavirus-govt-set-to-release-contact-tracking-app-which-detects-nearby-virus-carriers-11966243&sa=D&ust=1586111888580000)</span><span class="c7">,</span> <span class="c11 c10">[US](https://www.google.com/url?q=https://arxiv.org/pdf/2003.08567.pdf&sa=D&ust=1586111888580000)</span><span class="c7">,</span> <span class="c11 c10">[Germany](https://www.google.com/url?q=https://uk.reuters.com/article/uk-health-coronavirus-germany-tech/germany-aims-to-launch-singapore-style-coronavirus-app-in-weeks-idUKKBN21H275&sa=D&ust=1586111888580000)</span><span class="c7">, with one already deployed in</span> <span class="c11 c10">[Singapore](https://www.google.com/url?q=https://www.tracetogether.gov.sg/&sa=D&ust=1586111888580000)</span><span class="c7">. These apps have increasingly come under the spotlight as a potential long-term way to monitor the virus. Epidemiologists say that it could</span> <span class="c11 c10">[prove](https://www.google.com/url?q=https://science.sciencemag.org/content/early/2020/03/30/science.abb6936.full&sa=D&ust=1586111888581000)</span><span class="c7"> </span><span class="c11 c10">[vital](https://www.google.com/url?q=http://www.ox.ac.uk/news/2020-03-17-infectious-disease-experts-provide-evidence-coronavirus-mobile-app-instant-contact&sa=D&ust=1586111888581000)</span><span class="c7">to avoid long-term extreme confinement measures. The data handled by these apps, from</span> <span class="c11 c10">[location data](https://www.google.com/url?q=https://www.nytimes.com/interactive/2018/12/10/business/location-data-privacy-apps.html&sa=D&ust=1586111888581000)</span><span class="c7">to</span> <span class="c11 c10">[fine-grained close proximity information](https://www.google.com/url?q=https://privacyinternational.org/explainer/3536/bluetooth-tracking-and-covid-19-tech-primer&sa=D&ust=1586111888581000)</span><span class="c17 c7"> and whether a person might be infected and should self-quarantine is however very sensitive.</span>

<span class="c7">In</span> <span class="c11 c10">[our Mar 21 blog post](https://www.google.com/url?q=https://cpg.doc.ic.ac.uk/blog/fighting-covid-19/&sa=D&ust=1586111888582000)</span><span class="c7">, we emphasized how we do not have to</span> <span class="c11 c10">[pause privacy laws and regulations](https://www.google.com/url?q=https://www.nytimes.com/2020/03/24/business/coronavirus-medical-supplies-regulations.html&sa=D&ust=1586111888582000)</span><span class="c17 c7"> and how privacy engineering can help measure and limit the spread of the virus without resorting to mass surveillance.</span>

<span class="c7">When it comes to contact tracing, this however requires to go beyond simple reassurances that the phone numbers aren’t recorded, that everything is encrypted, that pseudonyms are changing, or that the app is based on consent. Indeed, a large range of techniques exist to circumvent those protections. For instance,</span> <span class="c11 c10">[scores](https://www.google.com/url?q=http://www.cs.columbia.edu/~mani/pub/RiedererWWW2016.pdf&sa=D&ust=1586111888582000)</span><span class="c7">have been developed to re-identify individuals in</span> <span class="c11 c10">[location](https://www.google.com/url?q=https://www.nature.com/articles/srep01376&sa=D&ust=1586111888582000)</span><span class="c7">or</span> <span class="c11 c10">[graph](https://www.google.com/url?q=https://arxiv.org/abs/0903.3276&sa=D&ust=1586111888582000)</span><span class="c7"> </span><span class="c11 c10">[datasets](https://www.google.com/url?q=https://arxiv.org/abs/1408.1276&sa=D&ust=1586111888582000)</span><span class="c7">,</span> <span class="c11 c10">[session fingerprinting](https://www.google.com/url?q=https://www.hindawi.com/journals/scn/2018/7352030/&sa=D&ust=1586111888582000)</span><span class="c7">could be used to link a pseudonymous app user to an authenticated web visitor, and node-based intrusions would allow to</span> <span class="c11 c10">[track users](https://www.google.com/url?q=https://cpg.doc.ic.ac.uk/blog/cambridge-analytica-is-only-the-beginning/&sa=D&ust=1586111888583000)</span><span class="c17 c7">.</span>

<span class="c17 c7">Apps are being developed around the world and are likely to be available within weeks. If they are proven useful, governments, health authorities, and users will have to evaluate the different approaches and decide whether to adopt them.</span>

<span class="c17 c7">Privacy is a crucial component in the equation. In this post, we propose 8 questions one should ask to assess privacy in contact tracing apps.</span>

## <span class="c6">Contact tracing – Setup</span>

<span class="c17 c7">We here focus on contact tracing apps installed by users and empowering them: apps informing users that they have been in close proximity with an infected individual in the past and providing them with recommendations on what to do.</span>

<span class="c17 c7">The privacy setting for such an app typically involves the following entities:</span>

*   <span class="c17 c7">Users who install the app on their phone;</span>
*   <span class="c17 c7">Authority (e.g. the government or a healthcare provider) that runs a central server coordinating the contact tracing;</span>
*   <span class="c17 c7">External entities: malicious apps, users, a foreign agency, or a company who is trying to take advantage of the situation to collect data or tamper with the contact tracing.</span>

<span class="c7">We use</span> <span class="c7 c30">user</span><span class="c7">to refer to anyone using the app,</span> <span class="c7 c30">infected</span><span class="c7">for users who have been tested and were found to be positive, and</span> <span class="c7 c30">at risk</span><span class="c17 c7"> for users who have been in close contact with someone who was later found to be infected.</span>

<span class="c7">A digital contact tracing app would typically work like this: Bluetooth signals or location information are recorded by phones; when a user is diagnosed positive (</span><span class="c7 c30">infected</span><span class="c7">), they upload their data (under some form) to the authority, which then arranges for other users to learn that they are</span> <span class="c7 c30">at risk</span><span class="c17 c7"> because they interacted with an infected person.</span>

<span class="c17 c7">To illustrate the vulnerabilities our questions are meant to surface, we use three “toy” protocols. Note that they are only meant to illustrate the questions and are not complete, deployable solutions for contact tracing, nor even good protocols.</span>

### <span class="c19">Toy protocol 1 (using location):</span>

*   <span class="c17 c7">Each app only records its own location.</span>
*   <span class="c17 c7">When a user reports as infected, they send their trajectory (location and time) to the authority.</span>
*   <span class="c17 c7">The authority shares the pseudonymous trajectories of all infected users with every user. Users can then check if they were in close contact with an infected individual.</span>

### <span class="c19">Toy protocol 2 (using Bluetooth):</span>

*   <span class="c17 c7">Each app broadcasts a unique identifier assigned by the authority through Bluetooth.</span>
*   <span class="c17 c7">When two phones are near to one another, they exchange these identifiers.</span>
*   <span class="c17 c7">When a user reports as infected, they send all the identifiers they encountered to the authority.</span>
*   <span class="c17 c7">The authority contacts all the users whose identifier was encountered by an infected user.</span>

### <span class="c19">Toy protocol 3 (using Bluetooth):</span>

*   <span class="c17 c7">Each app broadcasts a unique identifier using Bluetooth, assigned by the authority. This unique identifier is reset every hour.</span>
*   <span class="c17 c7">When two phones are near to one another, they exchange these identifiers.</span>
*   <span class="c17 c7">When a user reports as infected, they send all the identifiers that they have used (one per hour) to the authority.</span>
*   <span class="c17 c7">The authority shares the identifiers of all infected users with every user. Users can then check if they encountered one of these identifiers recently.</span>

<span class="c17 c7">Using this vocabulary and definitions, we propose 8 privacy questions that we would like app developers to answer. We hope these questions will help start a high-level discussion to systematically evaluate potential vulnerabilities and real risks in existing and future contact tracing apps.</span>

## <span class="c6">The questions</span>

<span class="c17 c7"></span>

### <span class="c19">1\. How do you limit the personal data gathered by the authority?</span>

<span class="c27 c7">Large-scale collection of personal data can quickly lead to mass surveillance.</span>

<span class="c7">In protocol 1, the authority learns the whole trajectory of infected users. In protocol 2, the authority learns the entire pseudonymous social graph of infected users, along with timestamps, which has been</span> <span class="c11 c10">[shown to be easily re-identifiable](https://www.google.com/url?q=https://arxiv.org/abs/0903.3276&sa=D&ust=1586111888588000)</span><span class="c17 c7">. Both collect large amounts of personal data. Protocol 3 does better in that regard, with the authority only observing the pseudonyms of infected users (with changing identifiers).</span>

### <span class="c19">2\. How do you protect the anonymity of every user?</span>

<span class="c27 c7">Users’ identities should be protected. Special measures should be put in place to limit the risk that users can be re-identified by the authority, other users, or external parties.</span>

<span class="c7">Protocol 1 doesn’t technically give the authority the identity of users. However,</span> <span class="c11 c10">[research](https://www.google.com/url?q=https://www.nature.com/articles/srep01376&sa=D&ust=1586111888588000)</span><span class="c7">shows that location traces are highly unique, and could probably be easily linked back to a person. Protocol 2 is worse, as the users are given a unique identifier by the authority, which can link these identifiers to the phone. Protocol 3 is much better – as long as connections with the server are anonymous (e.g. using</span> <span class="c11 c10">[Tor](https://www.google.com/url?q=https://apps.dtic.mil/dtic/tr/fulltext/u2/a465464.pdf&sa=D&ust=1586111888589000)</span><span class="c7">or</span> <span class="c10 c11">[mixes](https://www.google.com/url?q=https://dl.acm.org/doi/pdf/10.1145/358549.358563&sa=D&ust=1586111888589000)</span><span class="c17 c7">), the user’s identity could be kept secret.</span>

### <span class="c19">3\. Does your system reveal to the authority the identity of users who are at risk?</span>

<span class="c7 c27">The goal of contact tracing is to let people know they have been in contact with someone who was infected. The authority should not know who these people are.</span>

<span class="c17 c7">No for protocols 1 and 3, which never require data from non-infected users. Yes for Protocol 2, in which the authority explicitly contacts at risk users, and could use this information to, e.g., force them into quarantine.</span>

### <span class="c19">4\. Could your system be used by users to learn who is infected or at risk, even in their social circle?</span>

<span class="c27 c7">Having been in contact and infecting someone may become a matter of life and death. Digital contact tracing should warn people at risk without revealing who might have infected them.</span>

<span class="c17 c7">Protocol 1 exposes the full data of infected users publicly: every user can then check if a particular person they know is in the dataset. In protocol 3, a user at risk learns the hour at which they met an infected user, and can probably find out who infected them. Protocol 2, on the other hand, prevents users from learning anything about one another.</span>

### <span class="c19">5\. Does your system allow users to learn any personal information about other users?</span>

<span class="c27 c7">Apps should not need to leak information on a user’s locations or social networks to other users.</span>

<span class="c17 c7">All three protocols protect data of non-infected users, but only protocol 2 prevents users from learning anything about infected users. Protocol 1 exposes their entire trajectory. Protocol 3 leaks small amounts of information: identifiers encountered by infected individuals. It is possible for a user to recognize identifiers they have encountered and learn that the user to whom the identifier belongs is at risk.</span>

### <span class="c19">6\. Could external parties exploit your system to track users or infer whether they are infected?</span>

<span class="c27 c7">The system should take into account the risk of external adversaries, including well-resourced ones.</span>

<span class="c7">Both protocols 2 and 3 force phones to broadcast an identifier. An entity could install Bluetooth trackers to cover a city, or install malicious code on phones, and record the identifiers that they observe in specific locations. In</span> <span class="c11 c10">[our](https://www.google.com/url?q=https://arxiv.org/abs/1803.09007&sa=D&ust=1586111888590000)</span><span class="c7"> </span><span class="c11 c10">[research](https://www.google.com/url?q=https://cpg.doc.ic.ac.uk/blog/cambridge-analytica-is-only-the-beginning/&sa=D&ust=1586111888591000)</span><span class="c17 c7">, we showed that trackers installed on the phones 1% of London’s population would allow an attacker to track the real-time location of over half of the city. Protocol 3 makes this attack much more difficult, as the identifiers change every hour.</span>

### <span class="c19">7\. Do you put in place additional measures to protect the personal data of infected and at risk users?</span>

<span class="c27 c7">The system design may require revealing more personal information about users who are infected or exposed. But these are often the people who are more vulnerable and at risk.</span>

<span class="c17 c7">Protocol 1, and to some extent protocols 2 and 3, require infected users to share more data. Users at risk are however safe in protocol 1 and 2, but not in protocol 3, where some of the identifiers that they have used are published.</span>

### <span class="c19">8\. How can we verify that the system does what it says?</span>

<span class="c27 c7">Large-scale contact tracing is too sensitive to rely on blind trust. Transparency is essential to prove that the app functions as advertised.</span>

<span class="c7">Transparency of the full system is absolutely fundamental to guarantee privacy. This requires open protocol specifications, but also public source code,</span> <span class="c11 c10">[reproducible builds](https://www.google.com/url?q=https://signal.org/blog/reproducible-android/&sa=D&ust=1586111888592000)</span><span class="c7 c17">, and verifiability of what is being broadcasted by apps.</span>

* * *

<span class="c17 c7"></span>

<span class="c17 c7">In the next few weeks, most of us are likely to install a contact tracing app to help slow down the spread of coronavirus. The questions we propose here represent a starting point for an informed conversation on the privacy risks of apps we are being offered.</span>

<span class="c17 c7">Importantly though, they cannot replace a full independent privacy audit. In-depth formal analysis of the protocol is necessary before deployment and should be published. Protecting privacy should rely on mathematical proofs of correctness, with mitigation strategies considered only when necessary. Our questions focus on privacy aspects, but ensuring security is similarly crucial. This means, for example, supervising the integrity and authenticity of the crowdsourced data, evaluating how mobile malware could affect the app’s behavior, or assessing the resilience of the authority’s servers against intrusions.</span>

<span class="c17 c7">Building a contact tracing app that allows all of us to participate in the fight against COVID19 is possible, but it will require us to go beyond shallow reassurances that privacy is protected.</span>

<span class="c11 c10">[PDF version](https://www.google.com/url?q=https://cpg.doc.ic.ac.uk/blog/pdf/evaluating-contact-tracing-apps-here-are-8-privacy-questions-we-think-you-should-ask.pdf&sa=D&ust=1586111888592000)</span>
