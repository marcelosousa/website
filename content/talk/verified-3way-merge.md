---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Verified Tree-Way Program Merge"
subtitle: ""
summary: ""
authors: [Marcelo Sousa]
tags: []
categories: []
event: OOPSLA 2018
event_url: https://conf.researchr.org/track/splash-2018/splash-2018-OOPSLA
video: Video
video_url: https://www.youtube.com/watch?v=tWKOfczhlC0&list=PLyrlk8Xaylp4hRBrMJlov4fRy5YH8UgWu&index=4
date: 2018-11-09T13:30:00-05:00
lastmod: 2019-07-15T20:44:39+02:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---

Even though many programmers rely on 3-way merge tools to integrate changes from different branches, such tools can introduce subtle bugs in the integration process. This paper aims to mitigate this problem by defining a semantic notion of conflict-freedom, which ensures that the merged program does not introduce new unwanted behaviors. We also show how to verify this property using a novel, compositional algorithm that combines lightweight summarization for shared program fragments with precise relational reasoning for the modifications. Towards this goal, our method uses a 4-way differencing algorithm on abstract syntax trees to represent different program versions as edits applied to a shared program with holes. This representation allows our verification algorithm to reason about different edits in isolation and compose them to obtain an overall proof of conflict freedom. We have implemented the proposed technique in a new tool called SafeMerge and evaluate it on 52 real-world merge scenarios obtained from Github. The experimental results demonstrate the benefits of our approach over syntactic conflict-freedom and indicate that SafeMerge is both precise and practical.

Joint-work with Isil Dillig and Shuvendu Lahiri.
