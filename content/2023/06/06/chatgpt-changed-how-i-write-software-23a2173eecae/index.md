---
title: "ChatGPT 改变了我编写软件的方式"
date: 2023-06-06T16:57:34+08:00
updated: 2023-06-06T16:57:34+08:00
taxonomies:
  tags: 
extra:
  source: https://betterprogramming.pub/chatgpt-changed-how-i-write-software-23a2173eecae
  hostname: betterprogramming.pub
  author: Allen Helton
  original_title: "ChatGPT Changed How I Write Software - Better Programming"
  original_lang: en
---

## ChatGPT Changed How I Write Software  
ChatGPT 改变了我编写软件的方式

## Generative AI has completely changed the way I approach software design. I don’t think I could ever go back.  
生成式人工智能彻底改变了我进行软件设计的方式。我想我再也回不去了。

[

![Allen Helton][fig1]



](https://allenheltondev.medium.com/?source=post_page-----23a2173eecae--------------------------------)[

![Better Programming][fig2]



](https://betterprogramming.pub/?source=post_page-----23a2173eecae--------------------------------)

![Image by vectorjuice on FreePik][fig3]

AI is buzzing right now. All my social media feeds are about some new thing you can do with ChatGPT plugins or showing off a new photo created by generative AI. I’ll be honest, it’s pretty cool to see and I’m not mad about it.  
人工智能现在正在嗡嗡作响。我所有的社交媒体提要都是关于你可以用 ChatGPT 插件做的一些新事情，或者展示由生成式 AI 创建的新照片。老实说，看到它很酷，我对此并不生气。

The tech community seems to have gone on all-in on this AI gold rush. With new software, features, and enhancements popping up every day we have quickly found ourselves in a “sink or swim” moment. Do we embrace all the new advancements and see how development changes? Do we ignore it and hope it goes away? What about something in the middle?  
科技界似乎已经全力以赴地投入了这场人工智能淘金热。随着每天都有新的软件、功能和增强功能出现，我们很快就发现自己处于“沉没或游泳”的时刻。我们是否拥抱所有新的进步，看看发展如何变化？我们是否忽略它并希望它消失？中间的东西呢？

![Chart of the adoption bell curve][fig4]

_Photo by_ [_Jurgen Appelo_](https://www.flickr.com/photos/jurgenappelo/5201275209) 摄影：Jurgen Appelo

If we look at the adoption bell curve for AI above, I’d estimate we’re still somewhat at the beginning of the early adopter phase. Lots of people are making noise about it online, but not many of us are actually using it in production.  
如果我们看一下上面的AI采用钟形曲线，我估计我们仍处于早期采用者阶段的开始。很多人在网上对它大吵大闹，但我们中没有多少人真正在生产中使用它。

That said, AI’s time will come when it’s commonplace to see it in everything. It’s not something we’ll specifically notice, it will be assumed to be there and make software more delightful.  
也就是说，人工智能的时代将会到来，那时在所有事物中看到它都是司空见惯的。这不是我们会特别注意到的东西，它将被假定在那里并使软件更令人愉快。

Not for me, though. I’ve gone full swing into it and it’s taken over how I plan, design, and implement software. Granted, [I’m not an enterprise architect anymore](https://medium.com/@allenheltondev/8b74b92c573e), but I do run my website Ready, Set, Cloud by myself, and it has [a ton of software and services](https://medium.com/@allenheltondev/c3f2846c0bc) behind it that automate everything.  
不过，不适合我。我已经全力以赴，它接管了我如何规划、设计和实施软件。当然，我不再是企业架构师了，但我确实自己运行我的网站Ready，Set，Cloud，它背后有大量的软件和服务可以自动化一切。

I wanted to share how I approach application design now that I have incredibly powerful AI at my fingertips.  
我想分享我如何处理应用程序设计，因为我触手可及的强大人工智能。

## A Quick Foreword 快速前言

Before I go any further, we need to talk about a fallacy I’ve seen too many times drive technical and design decisions (and end up steering them away from innovation).  
在我进一步讨论之前，我们需要谈谈一个谬误，我已经见过太多次推动技术和设计决策（并最终引导他们远离创新）。

> There is no such thing as perfect software. The sooner you settle for “close enough” the sooner you and your customers will be happy.  
> 没有完美的软件。您越早接受“足够接近”，您和您的客户就会越早满意。

Don’t go into any design assuming you’re building the perfect software. Even if you designed it “perfectly”, when you go to implement it you’ll [go through several iterations](https://betterprogramming.pub/starting-over-with-purpose-my-serverless-adventure-99f0c051d73a) that end up changing it completely.  
不要假设您正在构建完美的软件进行任何设计。即使你设计得“完美”，当你去实现它时，你也会经历几次迭代，最终完全改变它。

It’s impossible to make everybody happy. People don’t need “perfect software.” They need something that _gets the problem done_.  
不可能让每个人都开心。人们不需要“完美的软件”。他们需要一些东西来完成问题。

With that in mind, I know AI isn’t perfect. It has hiccups. It might throw me a curveball every now and then. _That’s fine_. If I can solve a problem in a new innovative way that’s right 80% of the time, I’ve positioned myself for success.  
考虑到这一点，我知道人工智能并不完美。它有打嗝。它可能会时不时地给我一个曲线球。没关系。如果我能用一种新的创新方式解决问题，80%的时间都是正确的，我就已经为成功做好了准备。

Now that we have that out of the way, let’s talk about some new possibilities we have with the rapidly increasing availability of AI.  
现在我们已经解决了这个问题，让我们谈谈随着人工智能可用性的迅速增加，我们所拥有的一些新的可能性。

## New Possibilities 新的可能性

ChatGPT and other generative AI services out there have impressive pseudo-human capabilities. Questions that you’d normally have to prompt a human for can typically be answered by AI. If you’re willing to accept the answers given by these services (_and that’s a big IF_), you open the door to many more possibilities that would have required human interaction before.  
ChatGPT和其他生成AI服务具有令人印象深刻的伪人类能力。你通常必须提示人类的问题通常可以由人工智能回答。如果你愿意接受这些服务给出的答案（这是一个很大的假设），你就为更多的可能性打开了大门，而这些可能性以前需要人际互动。

## Data Transformations 数据转换

I wanted to create social media posts for my blogs when I publish them. I always do this manually but if given the chance, I would totally hand it off to a virtual assistant. I have the data from my blog post, but what I don’t have are the keywords, structure, and formatting that my target audience likes. I have a rough idea since I’ve been doing it for a while, but I’m never perfect.  
我想在发布博客时为我的博客创建社交媒体帖子。我总是手动执行此操作，但如果有机会，我会完全将其交给虚拟助手。我有博客文章中的数据，但我没有的是目标受众喜欢的关键字、结构和格式。我有一个粗略的想法，因为我已经做了一段时间，但我从来都不是完美的。

That said, ChatGPT can do it. It knows how to extrapolate information from my post and convert it specifically for a target audience. It has phenomenal information on market segments, and all I need to do to transform my data for a specific audience is just ask.  
也就是说，ChatGPT可以做到。它知道如何从我的帖子中推断信息并将其专门针对目标受众进行转换。它拥有关于细分市场的惊人信息，我需要做的就是为特定受众转换数据，只需询问即可。

“Create a Tweet about my content targeted at serverless developers based in the United States.”  
“创建一条关于我的内容的推文，面向位于美国的无服务器开发人员。”

If I wanted to target something else, I could ask it for a different variant, like “Create a LinkedIn post in Spanish from my blog post targeted at .NET engineers in Spain.”  
如果我想定位其他内容，我可以要求它提供不同的变体，例如“从我针对西班牙 .NET 工程师的博客文章中用西班牙语创建一篇LinkedIn文章”。

The response can simply be dropped into the Twitter API and sent along its way.  
响应可以简单地放入Twitter API并沿途发送。

## Data Generation 数据生成

This is probably the obvious one we already know. Give ChatGPT a prompt and have it generate data, an email, or a pdf of something. But it has such a wide range of use cases it’s worth stating the obvious.  
这可能是我们已经知道的显而易见的。给 ChatGPT 一个提示，让它生成数据、电子邮件或 pdf 的内容。但它有如此广泛的用例，值得一提。

I’ve blogged about [how I built a fitness app](https://medium.com/@allenheltondev/deda51878393) that generates workouts for me every day. I have a Lambda function that randomly decides which muscle group and gym equipment to use that day, and it creates a prompt to feed to ChatGPT. Then ChatGPT comes up with the entire workout, warmup, and cooldown for me to save to a database.  
我在博客上写了我如何构建一个健身应用程序，每天为我生成锻炼。我有一个 Lambda 函数，可以随机决定当天使用哪个肌肉群和健身器材，并创建一个提示以馈送到 ChatGPT。然后 ChatGPT 会为我提供整个锻炼、热身和冷却时间，让我保存到数据库中。

Prior to generative AI, this implementation would have been a nightmare. I would have needed some sort of database of exercises and ways to modify them for different types of workouts. Then I would have needed to come up with the logic that could modify them to pseudo-randomize and structure workouts. It would have been a multi-week build for subpar results.  
在生成式AI之前，这种实现将是一场噩梦。我需要某种练习数据库以及针对不同类型的锻炼进行修改的方法。然后我需要想出可以将它们修改为伪随机化和结构化锻炼的逻辑。这将是一个数周的构建，结果低于标准。

Instead, I spent 3 hours and built a Step Function workflow that queries ChatGPT and does all the heavy lifting for me (pun intended). I saved weeks of time leaning into AI instead of building something myself.  
相反，我花了 3 个小时构建了一个 Step Function 工作流来查询 ChatGPT 并为我完成所有繁重的工作（双关语）。我节省了数周的时间，而不是自己构建一些东西。

It doesn’t stop at workouts, you could [generate stories](https://aws.amazon.com/blogs/compute/implementing-an-event-driven-serverless-story-generation-application-with-chatgpt-and-dall-e/), build entire mock datasets from a provided schema, or come up with recipes with the food you have in your kitchen.  
它不会止步于锻炼，您可以生成故事，从提供的架构构建整个模拟数据集，或者根据厨房里的食物提出食谱。

But now, I can have meaningful data generated for me automatically with the right prompt. I go from “software engineering” to “prompt engineering”. You no longer need these massive databases of elements to feed custom business logic. Simply ask an LLM to use what it knows.  
但是现在，我可以通过正确的提示自动为我生成有意义的数据。我从“软件工程”到“提示工程”。您不再需要这些庞大的元素数据库来提供自定义业务逻辑。只需要求LLM使用它所知道的。

## Finding the Right Time 寻找合适的时间

Knowing when the right time to post content, react to an event, or send a notification is extremely difficult. Ideal times generally vary on a case-by-case basis and rarely fall into a generic configuration. A good example would be notifying on-call engineers when an anomaly is detected. You don’t want to notify on everything that pops up as it could introduce [alert fatigue](https://www.atlassian.com/incident-management/on-call/alert-fatigue).  
知道何时发布内容、对事件做出反应或发送通知的合适时间非常困难。理想时间通常因具体情况而异，很少属于通用配置。一个很好的例子是在检测到异常时通知值班工程师。您不想通知弹出的所有内容，因为它可能会引入警报疲劳。

If you routinely pass in a dataset to AI, it can identify anomalies and watch to see if it settles or even reason why the anomaly occurred in the first place. You can provide the AI some guidelines to only alert when something needs attention if it meets a certain set of criteria. This ultimately increases the effectiveness of your on-call crew and lowers your TCO purely based on manpower.  
如果你经常将数据集传递给人工智能，它可以识别异常并观察它是否解决，甚至解释异常首先发生的原因。您可以为 AI 提供一些准则，以便在满足一组特定条件时才需要注意时才发出警报。这最终会提高待命人员的效率，并纯粹基于人力降低您的 TCO。

You can also pass JSON objects to ChatGPT and ask for JSON in return. Let’s work through another example: _employee notifications_.  
你也可以将JSON对象传递给ChatGPT，并要求JSON作为回报。让我们通过另一个示例：员工通知。

With many people working from home nowadays, it’s impossible to generically send a message at a time that works for everyone. So you could use ChatGPT to identify activity trends of an individual to get a statistically high likelihood of reaching them online. Imagine this audit history:  
如今，许多人在家工作，因此不可能在适合所有人的时间发送消息。因此，您可以使用 ChatGPT 来识别个人的活动趋势，以获得在线联系他们的统计高概率。想象一下这样的审核历史记录：

```
[  {    "timestamp": "2023-05-26T14:52:21Z",    "event": "login"  },  {    "timestamp": "2023-05-27T16:40:09Z",    "event": "logout"  },  {    "timestamp": "2023-05-28T07:55:13Z",    "event": "login"  },  {    "timestamp": "2023-05-28T19:30:10Z",    "event": "logout"  }  // more audit events]
```

You can feed the audit history to ChatGPT, then provide it a prompt of:  
您可以将审核历史记录提供给 ChatGPT，然后为其提供以下提示：

> Return a json object with a “sendAtTime” property in ISO-8601 format that has the highest likelihood of reaching the person the next time they are online.  
> 返回具有 ISO-8601 格式的“sendAtTime”属性的 json 对象，该对象最有可能在下次联机时到达该用户。

This results in a response of:  
这会导致以下响应：

```
{  "sendAtTime": "2023-05-29T15:20:55Z"}
```

And you didn’t have to build an entire notification system! You pass in an audit history and ask generative AI to find the next time they will be online based on trends. It’s just so fast to build things that previously took weeks of careful time, planning, and effort. Now you can build a Step Function workflow that loads audit history, hits a [Lambda function to query ChatGPT](https://medium.com/@allenheltondev/d667e5b26d04), then set up a one-time EventBridge schedule.  
而且您不必构建整个通知系统！您传入审核历史记录，并要求生成 AI 根据趋势查找它们下次在线的时间。构建以前需要数周仔细时间、计划和精力的东西是如此之快。现在，您可以构建一个步骤函数工作流，该工作流加载审计历史记录，命中 Lambda 函数以查询 ChatGPT，然后设置一次性事件桥计划。

## How This Changes Development  
这如何改变发展

With all the examples we looked at before, a whole new set of use cases have unlocked. I no longer focus on building mundane systems that track CRUD operations. We have hundreds of examples that do that.  
通过我们之前看到的所有示例，一组全新的用例已经解锁。我不再专注于构建跟踪 CRUD 操作的平凡系统。我们有数百个例子可以做到这一点。

Instead, I now approach software with eye toward artificial reasoning. What can I ask ChatGPT that will take the most code out of my hands? I’ve gone on record a few times stating that [code is a liability](https://betterprogramming.pub/skip-the-lambda-function-connect-directly-to-your-aws-services-5f10798f2d5a). Any opportunity I have to take away code, I do it. This used to be in the way of directly connecting API Gateway to different AWS services. I would remove Lambda function code by skipping it altogether.  
相反，我现在着眼于人工推理来对待软件。我能问 ChatGPT 什么，它会从我手中拿走最多的代码？我已经记录了几次，指出代码是一种负担。只要有机会，我就拿走代码，我就去做。这曾经是将 API 网关直接连接到不同的 AWS 服务的方式。我会通过完全跳过来删除 Lambda 函数代码。

But now, I might not even need an endpoint to do what I want. Things can just… happen.  
但是现在，我甚至可能不需要端点来执行我想要的操作。事情可以只是...发生。

I approach development from a stance of “_what can I automate, where can I gather insights, and when should I act_” when data is created. Let’s take my blog as an example.  
在创建数据时，我从“我可以自动化什么，我可以在哪里收集见解，以及何时应该采取行动”的立场来处理开发。让我们以我的博客为例。

All my posts are saved as Markdown files in GitHub. When I push a new article to the `main` branch, a slew of activities occur:  
我所有的帖子都保存在GitHub中的Markdown文件。当我将新文章推送到 `main` 分支时，会发生一系列活动：

-   [Cross-post the content](https://allenheltondev.medium.com/aa4c6979ff9b) on other blogging platforms  
    在其他博客平台上交叉发布内容
-   Summarize and gather analytics on the article details  
    总结和收集对文章详细信息的分析
-   Synthesize a text-to-speech recording and save it back to the article  
    合成文本到语音转换录制并将其保存回文章
-   [Create writer analytics](https://medium.com/@allenheltondev/94d4ab0435ba) (writing skill level, tone, expertise in area, topics)  
    创建作家分析（写作技能水平、语气、领域专业知识、主题）
-   Identify the target and tangental audiences based on the content  
    根据内容确定目标受众和切线受众
-   Write social media posts targeting identified audiences summarizing the article content  
    针对已确定的受众撰写社交媒体帖子，总结文章内容
-   Schedule social media posts to go out at optimal times given the target audiences  
    根据目标受众安排社交媒体帖子在最佳时间发布

Now, some of this doesn’t exist yet — but it will thanks to generative AI. If you look at some of the actions that happen, ChatGPT is basically becoming an automated marketing team. Identifying the people a post would resonate with most, knowing how to reach out to them, and sending them tailored messages when they’re online are all marketing tasks — and hard ones at that!  
现在，其中一些还不存在 - 但它将归功于生成AI。如果你看看发生的一些行动，ChatGPT基本上正在成为一个自动化的营销团队。确定帖子最能引起共鸣的人，知道如何与他们联系，并在他们在线时向他们发送量身定制的消息都是营销任务——而且很难！

But because of the new way I’ve started approaching software development, this is all possible. I’m not looking into “how can I build a system that does X, Y, or Z”, I’m figuring out what I need to ask AI to do it for me.  
但是由于我开始进行软件开发的新方式，这一切都是可能的。我不是在研究“我怎样才能建立一个执行X，Y或Z的系统”，我正在弄清楚我需要让AI为我做什么。

It truly is a game-changer and all things considered, a [dirt-cheap option](https://openai.com/pricing#language-models) when it comes to ROI. Yes, the answers aren’t always perfect, but I’m ok with that. If I’m being honest, it’s never perfect when I build a solution by hand. But I’ve accelerated my time to completion by 100x, and that’s worth every penny.  
它确实是一个游戏规则改变者，考虑到所有因素，在投资回报率方面是一个非常便宜的选择。是的，答案并不总是完美的，但我对此没意见。老实说，当我手工构建解决方案时，它永远不会完美。但是我已经将完成时间加快了 100 倍，这值得每一分钱。

Happy coding! 祝您编码愉快！

[fig1]: 1ifG4msqzs8x1wQxrsjbIqQ.jpeg
[fig2]: 1QNoA3XlXLHz22zQazc0syg.png
[fig3]: 03OsUtsnlTx9Svm4c.jpg
[fig4]: 0qyDPvszYwph3Cwo1.jpg
