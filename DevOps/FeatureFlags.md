
Feature Flag/Toggle Resources
====

### Some Definitions:
* https://en.wikipedia.org/wiki/Feature_toggle
  * "A feature toggle (also feature switch, feature flag, feature flipper, conditional feature, etc.) is a technique in software development that attempts to provide an alternative to maintaining multiple source-code branches (known as feature branches), such that a feature can be tested even before it is completed and ready for release. Feature toggle is used to hide, enable or disable the feature during run time. For example, during the development process, a developer can enable the feature for testing and disable it for other users."
  * "Continuous release and continuous deployment provide developers with rapid feedback about their coding. This requires the integration of their code changes as early as possible. Feature branches introduce a bypass to this process. Feature toggles are an important technique used for the implementation of continuous delivery."
  * "The technique allows developers to release a version of a product that has unfinished features. These unfinished features are hidden (toggled) so they do not appear in the user interface. This allows many small incremental versions of software to be delivered without the cost of constant branching and merging. Feature toggles may allow shorter software integration cycles. A team working on a project can use feature toggle to speed up the process of development, that can include the incomplete code as well."



### Introductory Articles: Concepts
* https://martinfowler.com/articles/feature-toggles.html
  * "The basic idea is to have a configuration file that defines a bunch of toggles for various features you have pending. The running application then uses these toggles in order to decide whether or not to show the new feature."
* [Armory.io - Feature Flags vs Canaries](https://blog.armory.io/feature-flags-vs-canaries/)
  * "Feature flags expose a specific feature to a sample set of users and then measures it’s impact. Canaries expose a specific version of the entire application to a sample set of users and then measures it’s impact."
  * Feature Flags
    * "Generally used for user visible features"
    * "Great for well defined user experiments which span longer periods of time"
    * "Testing against cohorts of users (i.e. testing features by location, registration date, etc)"
    * "Becomes harder to test over time as more feature flags means more permutations of code paths"
    * "Adds additional overhead to engineers to remember to add flags, turn them on, measure results, and then turn them off when needed"
    * "Not possible to test on code changes that affect large portions of the code base"
  * Canaries
    * "Gives you information about every release that goes out"
    * "Spans a single deployment which is typically shorter than a feature/user experiment"
    * "Works well when you ship small diffs and are quickly changing production code"
    * "Almost no overhead when process is fully automated"
* https://weblogs.asp.net/fredriknormen/merge-hell-and-feature-toggle




### Caveats:
* Feature Flags/Toggles ARE TECHNICAL DEBT (!!)
* Beware Feature Flag Hell
* Increases Testing Complexity 
* Harder to Debug, Test, Support 
* [Feature Flags Are Flawed: Let's Make Them Better](https://www.slideshare.net/StephenYoung6/feature-flags-are-flawed-lets-make-them-better-dpc?qid=722f4a70-ec48-41da-a5d4-93a664f0754d&v=&b=&from_search=14)
* [Knightmare: A DevOps Cautionary Tale](https://dougseven.com/2014/04/17/knightmare-a-devops-cautionary-tale/)
* [Feature Toggles are one of the Worst kinds of Technical Debt ](https://dzone.com/articles/feature-toggles-are-one-worst)
  * "The plumbing and scaffolding logic to support branching in code becomes a nasty form of technical debt, from the moment each feature switch is introduced. Feature flags make the code more fragile and brittle, harder to test, harder to understand and maintain, harder to support, and less secure. "
  * "should only be a temporary deployment/release management tool, and describes a disciplined lifecycle that all feature toggles need to follow, from when they are created by development, then turned on by operations, updated if any problems or feedback come up, and finally retired and removed when no longer needed."
  * "Feature toggles require a robust engineering process, solid technical design and a mature toggle life-cycle management. Without these 3 key considerations, use of feature toggles can be counter-productive. Remember the main purpose of toggles is to perform release with minimum risk, once release is complete toggles need to be removed."
  * Guiding Principles:
    * "Minimize your use of feature flags for release management"
    * "Review flags often, make sure that you know which flags are on and which are supposed to be on and when features are going to be removed."
    * "Once a feature is part of mainline, be ruthless about getting it out of the code base as soon as it isn't used or needed any more."
    * "Recognize and account for the costs of using feature flags, especially long-lived business logic branching in code."
* [2017, Martin McKay: Martin Fowler and feature branches revisited](https://jamesmckay.net/tag/feature-switches/)
  * [2011, Martin McKay: Why does Martin Fowler not understand feature branches?](http://web.archive.org/web/20110721063430/http:/jamesmckay.net/2011/07/why-does-martin-fowler-not-understand-feature-branches/)
* [Don‘t run with Feature Toggles in your hands](https://serialseb.com/blog/2016/01/26/dont-run-with-feature-toggles-in-your-hands/)




### Useful Refernces
* http://featureflags.io/feature-flags/



### Frameworks/Tooling
* http://enterprisedevops.org/feature-toggle-frameworks-list/
* https://launchdarkly.com/
  * https://try.launchdarkly.com/feature-toggle/
  * https://launchdarkly.com/benefits/
  * https://launchdarkly.com/pricing/
    * $75/mo for one developer
    * $325/mo for five developers 
    * contact sales, for more info 
    * Used by:
      * Atlassian, Microsoft, Meetup, GoDaddy, QVC, PluralSight, ...
  * [Implementing Feature Flags in an Angular E-commerce App](https://launchdarkly.com/blog/implementing-feature-flags-in-an-angular-e-commerce-app/)
* Split.io 
  * https://www.split.io/
  * https://www.split.io/product/feature-flags/
    * "Split solves the feature flag gap. And, Split goes beyond simple on/off feature toggling, providing granular targeting capabilities to expose a feature to exactly the right users, based on any attribute and with sophisticated regex matching. This enables more comprehensive feature management and gives product teams the flexibility to ensure exactly the right user experience."
    * https://www.split.io/pricing/
      * Starts at $700/month, up to 5 developers
* Hobknob 
  * https://github.com/opentable/hobknob 
    * "Hobknob is a feature toggle front-end built on top of etcd. It allows users to create and modify feature toggles, which can then be accessed in your applications"
    * "Features in Hobknob are grouped by application. Each application can have many, uniquely named features. Each feature will either have one on/off toggle or many on/off toggles (see Categories below). This gives us a simple way to identify toggles - ApplicationName/FeatureName[/SecondaryKey]."
    * "Hobknob has the concept of feature categories, where you can define secondary keys for each feature. This gives you the ability to set and get toggle values for App/Feature/SecondaryKey."
    * https://github.com/opentable/hobknob-client-net
      * A .net client library for Hobknob 
  * [Introducing Hobknob: Feature toggling with etcd](http://tech.toptable.co.uk/blog/2014/09/04/introducing-hobknob-feature-toggling-with-etcd/)
  * [Hobknob v2.0: A new dimension](http://tech.toptable.co.uk/blog/2014/11/26/hobknob-v2-dot-0-a-new-dimension/)
* Archaius (Netflix)
  * Doesn't appear to be very active, last commit was Nov 11, 2017...
  * https://github.com/Netflix/archaius
  * https://github.com/Netflix/archaius/wiki
  * https://github.com/Netflix/archaius/wiki/Features
  * https://medium.com/netflix-techblog/announcing-archaius-dynamic-properties-in-the-cloud-bc8c51faf675https://medium.com/netflix-techblog/announcing-archaius-dynamic-properties-in-the-cloud-bc8c51faf675
* Flagr
  * https://checkr.github.io/flagr/#/
  * https://github.com/checkr/flagr
    * "Flagr is an open source Go service that delivers the right experience to the right entity and monitors the impact. It provides feature flags, experimentation (A/B testing), and dynamic configuration. It has clear swagger REST APIs for flags management and flag evaluation." 
  * https://checkr.github.io/flagr/#/flagr_overview
  * https://engineering.checkr.com/introducing-flagr-a-robust-high-performance-service-for-feature-flagging-and-a-b-testing-f037c219b7d5
    * "Flagr makes the rollout process as easy as clicking buttons."
    * "Flagr supports feature flagging, A/B testing, and dynamic configuration. All of them are first class citizens in Flagr. Moreover, Flagr can run multi-variants experimentation, and you are not limited to binary on/off toggles."
    * "Flagr can target any audience. It uses rich constraints to define user segmentation. The scope is bigger than the traditional web feature toggles, and it’s flexible enough to flag requests from mobile apps, frontend, and backend systems."
    * "Flagr logs data records and impressions, so it’s easy to build your own analytics at the feature level. It decouples the metrics computation from flag evaluation, and you own 100% of your data."


### Language Specific Tools...
* Java Programming
  * https://www.togglz.org/
* JavaScript Programming
  * https://github.com/bigodines/feature-flipper-js
    * NOTE: No longer being actively maintained
  * https://www.npmjs.com/package/angular-feature-toggle
  * https://github.com/michaeltaranto/angular-feature-flags
    * NOTE: No longer being maintained, last commit, July 26, 2017 
    * "An AngularJS module that can be used to hide/exclude application features until they are ready."
  * https://www.npmjs.com/package/ngx-feature-toggle
    * https://github.com/willmendesneto/ngx-feature-toggle
  * Swivel
    * NOTE: Doesn't appear to be actively maintained, last commit, Oct 9, 2017
    * https://github.com/zumba/swivel
* .NET Programming 
  * https://github.com/jason-roberts/FeatureToggle
    * http://dontcodetired.com/blog/?tag=/featuretoggle
    * https://samueleresca.net/2017/01/feature-toggling-using-asp-net/
    * http://www.bousie.co.uk/blog/feature-toggling-for-pain-relief/ 


### Supplemental/Ancillary Tooling
* JSON Toggle
  * NOTE: proof-of-concept, for Java
  * https://github.com/whiskerlabs/toggle
  * https://evanm.website/2017/02/introducing-json-toggle/
* https://www.spinnaker.io/
  * https://www.spinnaker.io/concepts/
    * Spinnaker is an open-source, multi-cloud continuous delivery platform that helps you release software changes with high velocity and confidence."
    * "Spinnaker provides two core sets of features:"
      * "application management"
      * "application deployment"
* https://www.consul.io/
  * "Consul is a service mesh solution providing a full featured control plane with service discovery, configuration, and segmentation functionality. Each of these features can be used individually as needed, or they can be used together to build a full service mesh. Consul requires a data plane and supports both a proxy and native integration model. Consul ships with a simple built-in proxy so that everything works out of the box, but also supports 3rd party proxy integrations such as Envoy."
* Optimizely
  * https://blog.optimizely.com/2017/10/18/feature-management/


### Articles:
* [Infoq: Feature Toggles Revisited](https://www.infoq.com/news/2016/02/featuretoggles)
* https://rollout.io/blog/ultimate-feature-flag-guide/
* https://rollout.io/blog/top-5-use-cases-feature-flags/
* Angular related articles:
  * [https://blog.theodo.fr/2016/08/feature-toggling-in-angular-with-20-lines-of-code/](https://blog.theodo.fr/2016/08/feature-toggling-in-angular-with-20-lines-of-code/)
  * [Feature Toggling with Angular and the Angular CLI](https://medium.com/@amcdnl/feature-toggling-with-angular-and-the-angular-cli-eccf38369b3f)
  * [Integrating Feature Flags in Angular v4](https://blog.launchdarkly.com/integrating-feature-flags-in-angular-v4/))
  * [How To Use Angular Route Guards As Feature Toggles](https://www.technouz.com/4750/how-to-use-angular-route-guards-as-feature-toggles/)
  * [Feature Toggles for Angular UIs](https://www.linkedin.com/pulse/feature-toggles-angular-uis-adam-knight/)
  * https://rollout.io/blog/guide-feature-toggle-angular/
* https://appdevelopermagazine.com/using-feature-flags-in-your-app-release-management-strategy/
* [Decoupling Deployment and Release- Feature Toggles](https://www.abhishek-tiwari.com/decoupling-deployment-and-release-feature-toggles/)
  * "Term dark launching was coined by Facebook engineering team to simulate the new features in production environment well before release."
  * Uses:
    * "for avoiding branching and merging"
    * "experimenting such as A/B tests"
    * "putting unfinished code in production"
    * "reducing risk associated with large change"
    * "turning a resources heavy feature OFF in high load conditions"
    * "Once your start using feature toggles regularly, it is good idea to group the features"
    * "Feature toggles require a robust engineering process, solid technical design and a mature toggle life-cycle management. Without these 3 key consideration, use of feature toggles can be counter-productive."
* [O'Reilly.com - Implementing continuous delivery](https://www.oreilly.com/ideas/implementing-continuous-deliveryhttps://www.oreilly.com/ideas/implementing-continuous-delivery)
  * "The requirements for increased velocity and the associated modern architectural styles strongly encourage separating the process of deployment and release. This has ramifications for the way you design, test and continuously deliver software."
  * "One core approach to such deployment is the use of feature flags or ability to turn features (sub-sections) of your application on/off with ease. This allows you to continuously deploy new features, but control when they are released into production."
* .NET Related
  * [Feature toggles in .NET: tips and tricks](https://surfingthecode.com/feature-toggles-in-.net-tips-and-tricks/)
  * [.NET/C# Feature Flag Resources/Solutions](https://featureflags.io/dotnet-feature-flags/)
  * [Implementing Feature Toggles in .NET with Feature Toggle](https://www.pluralsight.com/courses/dotnet-featuretoggle-implementing)
  * [Implementing feature toggle in ASP.NET Core](https://dotnetthoughts.net/implementing-feature-toggle-in-aspnet-core/)
  * [InfoWorld: How to Implement a feature toggle in C#](https://www.infoworld.com/article/3241110/c-sharp/how-to-implement-feature-toggle-in-c-sharp.html)
  * [Microsoft: Explore how to progressively expose your features in production for some or all users](https://docs.microsoft.com/en-us/azure/devops/articles/phase-features-with-feature-flags?view=vsts)
  * [Microsoft DevOps Blog: Effective Patterns for Feature Flags](https://blogs.msdn.microsoft.com/devops/2016/06/24/effective-patterns-for-feature-flags/)
  * [Feature Toggle v4 RC1 with .NET Core Support](http://dontcodetired.com/blog/post/FeatureToggle-v4-RC1-with-NET-Core-Support)
  * [Dave's Daydreams blog: Feature Toggle libraries for .NET](https://david.gardiner.net.au/2012/07/feature-toggle-libraries-for-net.html)
  * [Microsoft: HOL - Feature Flag for Web Applications](https://microsoft.github.io/PartsUnlimited/advanced/FeatureFlagWeb.html)
  * [Simple Feature Toggles for Asp.Net Core](https://blog.vincentcos.tel/simple-feature-toggles-for-asp-net-core/)
* [https://minops.com/blog/2015/02/the-dos-and-donts-of-bluegreen-deployment/](https://minops.com/blog/2015/02/the-dos-and-donts-of-bluegreen-deployment/)
* [Slideshare.net - Feature Toggle, by Bryan Liu, DevOps Evangelist & Quality Engineer](https://www.slideshare.net/bryan0817/feature-toggle-64967183)
* [Feature Toggles (Feature Switches or Feature Flags) vs Feature Branche](https://technologyconversations.com/2014/08/26/feature-toggles-feature-switches-or-feature-flags-vs-feature-branches/)
* [Continuous Delivery Using Feature Togggles](https://samueleresca.net/2017/01/continuos-delivery-using-feature-toggle/)
* [Peter Morlin - Simple Feature Toggling](https://www.petermorlion.com/simple-feature-toggling/)
* [Pete Hodson - Feature Branching vs. Feature Flags: What’s the Right Tool for the Job?](https://devops.com/feature-branching-vs-feature-flags-whats-right-tool-job/)
* [Fun with Feature Flags](https://www.centric.eu/NL/Default/Craft/Blogs/2018/03/13/Fun-with-Feature-Flags)



### My Backlog to read: Still need to review/assess whether there's any value in these articles... 
* http://wiki.glitchdata.com/index.php/Feature_toggle
* https://blog.getambassador.io/deploy-and-release-decouple-for-speed-and-safety-a8c99a9b4d7b
* https://www.sitepoint.com/feature-toggling-explained-with-qandidates-toggle/
* https://willmendesneto.github.io/ngx-feature-toggle/index.html
* https://www.equinox.co.nz/blog/feature-toggles-on-net-core-api
* https://blog.objectivity.co.uk/feature-toggle/



### Use Cases / Case Studies:
* https://launchdarkly.com/use-cases/
* Netflix
  * https://launchdarkly.com/blog/tag/netflix/
  * https://medium.com/netflix-techblog/preparing-the-netflix-api-for-deployment-786d8f58090d
* Etsy
  * https://codeascraft.com/2011/02/04/how-does-etsy-manage-development-and-operations/ 
* Realtor.com
  * https://blog.optimizely.com/2018/10/23/realtor-com-better-customer-experience/
* Reddit
  * https://blog.optimizely.com/2018/10/12/ask-an-experimenter-kevin-chen-growth-pm-at-reddit/
* [2016 IEEE/ACM 13th Working Conference on Mining Software Repositories - Feature Toggles: Practitioner Practices and a Case Study](https://www.computer.org/csdl/proceedings/msr/2016/4186/00/07832900.pdf)
  * https://dl.acm.org/citation.cfm?id=2901745 
* AWS
  * [Continuous Delivery and Effective Feature Flagging with LaunchDarkly](https://aws.amazon.com/blogs/startups/continuous-delivery-and-effective-feature-flagging-with-launchdarkly/)
* Gitlab.com
  * https://docs.gitlab.com/ee/user/project/operations/feature_flags.html
* Pivotal Cloud Foundry (CF)
  * https://docs.pivotal.io/pivotalcf/1-12/adminguide/listing-feature-flags.html
    * "This topic describes how Cloud Foundry (CF) administrators can set feature flags using the Cloud Foundry Command Line Interface (cf CLI) to enable or disable the features available to users."
  * https://docs.cloudfoundry.org/adminguide/listing-feature-flags.html
* Google Chrome
  * [The Modular and Feature Toggle Architectures of Google Chrome](http://users.encs.concordia.ca/~pcr/paper/Rahman2018EMSE-preproduction.pdf)
* OpenLMIS
  * https://openlmis.atlassian.net/wiki/spaces/OP/pages/38371426/2.0+Feature+Toggle+Mechanism


### Slideshare.net
* Microsoft
  * [Lessons Learned Doing DevOps at Scale at Microsoft ](https://www.slideshare.net/BuckHodges/lessons-learned-doing-devops-at-scale-at-microsoft?qid=fc47221a-23fc-4a82-8a95-49e00023f18d&v=&b=&from_search=8)
* Upwork
  * [Feature Flags. Reducing risks during shipping changes/ ](https://www.slideshare.net/amahomet/feature-flags-reducing-risks-during-shipping-changes?qid=722f4a70-ec48-41da-a5d4-93a664f0754d&v=&b=&from_search=3)
* [Feature flags to speed up & de risk development ](https://www.slideshare.net/LaunchDarkly/feature-flags-to-speed-up-de-risk-development?qid=722f4a70-ec48-41da-a5d4-93a664f0754d&v=&b=&from_search=4)
* [Ship Faster, Reduce Risk, and Build Scale with Feature Flags](https://www.slideshare.net/GoAtlassian/ship-faster-reduce-risk-and-build-scale-with-feature-flags?qid=722f4a70-ec48-41da-a5d4-93a664f0754d&v=&b=&from_search=8)
* [Progressive exposure using deployment rings and feature flags](https://www.slideshare.net/WillyPeterSchaub/progressive-exposure-using-deployment-rings-and-feature-flags?qid=722f4a70-ec48-41da-a5d4-93a664f0754d&v=&b=&from_search=9)
* [TDC2018SP | Trilha UX - Feature flags e Releases controlados ](https://www.slideshare.net/tdc-globalcode/tdc2018sp-trilha-ux-feature-flags-e-releases-controlados?qid=722f4a70-ec48-41da-a5d4-93a664f0754d&v=&b=&from_search=11)
* [Adopting feature flags with Visual Studio Team Services (VSTS), Azure DevOps ](https://www.slideshare.net/VSTSCommunityMicroso/testing-in-production-with-feature-flags?qid=722f4a70-ec48-41da-a5d4-93a664f0754d&v=&b=&from_search=16)
* [DevOps West: Feature flags for Clean Deployments ](https://www.slideshare.net/LaunchDarkly/devops-west-feature-flags-for-clean-deployments?qid=722f4a70-ec48-41da-a5d4-93a664f0754d&v=&b=&from_search=19)
* [GlueCon 2016: Faster Feedback with Feature Flags ](https://www.slideshare.net/LaunchDarkly/gluecon-faster-feedback-with-feature-flags?qid=722f4a70-ec48-41da-a5d4-93a664f0754d&v=&b=&from_search=21)




### Videos / Podcasts:
* [GOTO 2017 • Feature Branches and Toggles in a Post-GitHub World • Sam Newman](https://www.youtube.com/watch?v=lqRQYEHAtpk)
  * Sam Newman - Author of "Building Microservices" from O'Reilly 
* [Dan Piessens presentation, DevOpsDays Chicago 2015 - It's More Than Feature Toggles](https://www.youtube.com/watch?v=G-3FOxesB14)
* [Feature toggles on an Angular UI - using the LaunchDarkly console](https://www.youtube.com/watch?v=mLu7LfqRTos)
* https://www.youtube.com/watch?v=cC7pQcNKQbc
* [InfoQ: Using Feature Flags](https://www.youtube.com/watch?v=WMRjj06R6jg)
* [What is a Feature Toggle?](https://www.youtube.com/watch?v=KooEz-3egzc)
* Microsft User Group
  * [DevOps at Speed with Feature Flags](https://www.youtube.com/watch?v=cC7pQcNKQbc)
* [.NET Rocks - Feature Toggles with Daniel Piessens)](https://player.fm/series/net-rocks/feature-toggles-with-daniel-piessens)


