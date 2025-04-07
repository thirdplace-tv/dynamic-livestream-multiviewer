This is a technical discussion of [Thirdplace.tv](https://www.thirdplace.tv), a new dynamic, spatial, livestream multiviewer that immerses the user in the world of livestreaming in a way never before possible, and which could also be the solution to remote work.

# Section I: Introduction

Look at these images, and think about what they have in common.

![Dual image, one of people in a coffeeshop, and one of people in a coworking space](/images/coffeeshop_and_coworking.png "Coffeeshop and Coworking Space")

We all know they have something intangible in common, but what?  I've tried to define it and failed every time. 	The closest term I've found for them is that they're all "shared spaces", but even that isn't quite right. 	Maybe there isn't a term for it, and isn't that strange?

The tech industry hasn't figured it out either.

They've give us social networks, content sharing services, video conferences, and other tools.

![Dual image, one of boring people singing in a Zoom meeting, and one of the muppets from The Muppet Show singing under arches](/images/zoom_muppets.png "Zoom Muppet Show")

But none of those are really shared spaces.  They're bulletin boards, they're stage shows, they're meetings.  But they're not *places*, they're not continuous, they're not alive.

They're not what we yearn for.  And they're not what we need.

Livestreaming seems close.  Livestreaming offers authentic human connection in a way that most other content does not.

But watching a livestream never feels like you're in a *shared space*.  It feels like you're in an audience at a show.

And browsing and exploring livestreams?  That feels like flipping through a TV Guide in 1983, trying to choose a channel to watch on a wood paneled TV by scanning text descriptions.

It doesn't feel right.

None of it feels right.

I wanted a persistent space *full* of authentic human connection, vibrant with social ambiance and endless possibilities, aligned with my interests, and with easy and powerful discoverability and personalization.

I couldn't find one.

So I made one.

Let me introduce you to what I call Thirdplace.  Click the image below to see a demo.

[![Watch the demo](/images/thirdplace_screenshot_play.png)](https://youtu.be/WP_2PuIDCzs)


# Section II: The Problem


The core problem with existing livestream browsing and viewing experiences is that they operate under paradigms built for static, one-at-a-time consumption. Watching a single stream feels isolating, as though you are part of an audience rather than within a shared space. Browsing streams feels like flipping through a TV Guide in 1983 — clunky, uninformative, and utterly incapable of dynamically surfacing content.

Come to think of it, the entire industry seems stuck in 1983.

Every livestreaming service lets you browse text descriptions of shows, and sometimes image previews, to choose something to watch — just like flipping through that 1983 TV Guide.  And once you pick a show, you click into it — just like clicking your wood-paneled TV over to a channel in 1983. Then you watch that show until you decide to stop, or it ends. And then you repeat the process.

That was a fine paradigm for the technical limitations of 1983, and for long-form entertainment content, where every second and frame is carefully planned, edited, and tuned to maximize a focused watching experience.

But this isn’t 1983.

And livestreams aren’t movies.

They’re chaotic, unpredictable, unplanned.  Half the time, they’re barely even content.  They feel more like spontaneous conversations in a coffeeshop, or emergent experiences in a college dorm, than anything on television in 1983.  And their chatrooms amplify that effect, adding a real and participatory social atmosphere.

So why do we treat them like 1983 TV content?  Did we give up?  Did we smile contentedly and pat ourselves on the back for adding a chatroom to a 1983 TV experience, in a medium that doesn't work anything like TV?

What if we got it all wrong?

What if we were supposed to go the other direction?

What if instead of improving on 1983, we imagined the distant future?  What's the extreme upper bound of this technology, instead of the lower bound?  The furthest step forward, rather than the closest?

If watching a stream has the social energy of a conversation in a coffeeshop, then why not build the rest of the coffeeshop?

And why not build an entire city around it?

People yearn for a sense of community.  They need shared spaces.  And technology isn’t offering them any.

So what if we did?

What if we figured out how to turn 100,000 concurrent livestreams into a living, breathing, and most importantly, personalized, virtual city?

Let's think about how we could try to do that.

We could try using a living feed of some kind, like TikTok but for livestreams, but Tiktok only works because of its short-form content that quickly ends and provides an opportunity to replace it with the next content.  That just doesn't work for long-form content.

We could try a scrollable browsing system, or maybe a fixed player and a browsable list of streams to click around, but it seems we have once again reinvented 1983 wood paneled televisions, we're just upgrading the TV Guide.  A faster way to choose and watch one livestream, but which would in no way feel like a coffeeshop much less a city.

In fact, no way to present one stream at a time feels right.  Streams have so much dead time and unexpected emergent surprises that where a TV show requires the viewer's full attention, streams instead benefit considerably from ambient attention.  Glancing over from time to time, listening to a low volume background stream, not watching with rapt attention.

This makes one stream at a time often unrewarding.

So let's try more than one stream.

A system that enables viewing more than one stream simultaneously could be called a "multiview".

So it seems we need a multiview, to present more than one stream, more than one participant, more than one point of view, more than one **soul**.  But within that multiview we'll need to be able to move our focus around however we like without losing sight of the other people and points of view in that space, just like looking around a coffeeshop or out the window while having a pleasant conversation.

And, like a coffeeshop, we should have active control over some areas in it, the areas we're sitting, the areas we're standing, the areas we invite our friends to sit or stand.  Meanwhile, other areas should be open for free and dynamic movement of visitors, people we haven't actively engaged with, but who hopefully share our interests and align well with us, based on passive signals of the space, the coffeeshop, the city.  The way a sign in the window, the name of the shop, an A-frame sign on the sidewalk advertising a discount for attendees of the local comic convention, all passively steer like-minded individuals into the open spaces in the shop.

Okay, so let's look at multiviews.

Multiviews are not new technology on their own.  We see them in camera-monitoring systems, we see them sometimes in service- or streamer-provided static displays, we see them in static online multiviewers where we type in channels or streams or videos to be displayed.

But none of these are right for our purposes.

Those existing solutions are designed for small, known inputs, like that fixed set of security feeds or the statically typed list.  They offer no built-in browsing or discovery, limited adaptive or spatial features, no dynamic personalization, and no way to gracefully handle thousands of unpredictable, ever-changing livestreams.  They aim at a stable, unchanging environment — completely unlike the chaotic, massive, user-driven world of livestreaming.

They're small classrooms with assigned seating and no windows or doors, not coffeeshops or chaotic college dorms.

Clearly, we need a completely new kind of solution.

Let’s look at what I came up with.



# Section III: How I Solved The Problem


I originally set out to make a dynamic livestream multiviewer as a learning exercise, thinking this was a fairly simple extension of existing static multiviewers.

Generally, in software, making something dynamic is often as simple as taking a static version and attaching it to a database.  Results become data-driven rather than predefined, and adding interfaces to create, update, and delete the data gives control over the system.  Sometimes these interfaces can be cleverly concealed behind smart UI's but the underlying mechanisms remain.

That plan did not survive contact with the enemy.

Not only was I wrong about it being a simple problem, I was wrong from top to bottom.  The current incarnation of Thirdplace doesn't even use a database, nor would it ever likely be primarily driven from one.

Instead, data arrives from external sources and in a kind of waterfall — chaotic, frequently updating, and at a nearly massive scale.

Thinking about "multiviewers" really didn't get me anywhere in addressing this problem.  I tried various approaches I'll outline in the detailed technical discussion below, but at each step I failed.  No current solutions were even close to what was needed, so I had nothing to iterate forward from, and decomposing the problem only generated a fractal network of subproblems that couldn't be adequately solved in isolation.

So instead, I looked at the problem backwards, starting at the end, with this question:

How do you turn a waterfall into a coffeeshop?

It turns out that this is not a trivial problem.

As I thought about it and looked for inspiration, I lucked into an interesting tidbit.

I've always loved reading, and I grew up reading all sorts of scifi and other fiction, including Tom Clancy thrillers.

So I've heard of something called a "SONAR waterfall display".

Submarines can't see very far through water, so they use SONAR as their eyes, listening passively to the ocean or sending active signals and analyzing the bounced data.  A combination of passive and active systems.

But, like me with livestreams, submarines need a way to visualize this chaotic and very peculiar form of data.

The way they visualize this data is through something called a waterfall display, which combines positional and temporal data from passive and active sources into a continuous living feed, sort of a moving chart where the Y axis is time starting with the present at top and going backward as you look down the screen, constantly updating so that the resulting display appears to continuously scroll down (the "waterfall").  The X axis is bearing from the submarine's position, in 360 degrees.  And data points on the display are colored according to SONAR returns, with different brightnesses indicating different noise levels.  At a glance, you can see trends over time of noise sources "moving" directionally, popping up and/or vanishing, and static noise levels staying constant.  It's quite a remarkable solution.

I was particularly interested in how many of those elements overlap with shared spaces like coffeeshops; positional and temporal data, the combination of passive and active factors and influences, multiple inputs merged into a single continuous living experience, chaos made comfortable.  I knew that this was conceptually similar to the solution I would need for my dynamic multiviewer, even if the practical solution would look completely different.

Two things seemed apparent from that thought experiment:

1. You cannot turn a waterfall into a coffeeshop with a dozen loosely coupled features flying in close formation.  It's not a question of adding independent plugins or capabilities.  Instead, like the waterfall display, the solution will only work as a tighly integrated system of interlocking elements, where the removal of even one necessary element dooms the entire enterprise.

2. I understood technology pretty well, but it turns out that I did not understand shared spaces well at all.  In fact, I'm not sure anyone does.  We think we understand shared spaces because we thrive in them.  Just like we think we understand walking.  So simple a toddler can do it.  But when we try to teach a robot to walk, we realize we don't understand it at all.  So too with shared spaces.

We've all been in coffeeshops.  Many of us have been in college dorms, LAN parties, conventions, conferences, or open offices.  We know those spaces work.  But WHY those spaces work - that’s something we rarely think about, let alone understand deeply enough to recreate digitally.

So part of this invention wasn’t just about solving a technical problem.  It was about realizing that nobody had ever solved this deeper problem - or maybe even recognized it - and only then figuring out how to solve it.

And that’s how I arrived here.

What I describe in this document is a system for turning a waterfall into a coffeeshop — for turning a massive, shifting flood of livestreams into a persistent, dynamic, personalized shared space that feels alive, responsive, vibrant yet comfortable, and human.

At its core, the system weaves together a persistent multiview, an ongoing stream data pipeline, dynamic sorting and filtering that integrates both passive and active positioning elements, spatial and audio management, interactive elements, and a whole suite of additional mechanisms, that collectively preserve continuity and immersion even as every part of the system shifts and changes beneath the user’s feet, creating a spatial experience that carefully and thoughtfully merges vibrant dynamic elements with constant familiar elements, mirroring the delightful benefits of physical shared spaces.

Even that paragraph is an oversimplification, being neither exhaustive nor limiting.  This is a difficult system to describe, because it didn't arise from a description.  It arose from a problem, which nobody seems to have ever solved, and which few seem to have tackled at all.

So let me start talking about the problems and how they shaped the overall solution.

I will try explain each piece of the system in detail — how it works, how it connects to the others, and why it is necessary to the whole.  I will also try to document optional or implementation-specific features that play their own roles.


# Section IV: The Core Multiview


We've established that we need a multiview, but we haven't talked about exactly what constitutes one.  And our specific requirements go considerably beyond a simple implementation.

In a real coffeeshop or dorm lounge, multiple conversations happen at once.  But people also come and go, and move around.  And yet, no matter the movements, the space itself feels continuous — no one tears down the entire building every time someone leaves or enters. This “shared space” feeling demands a multiview capable of not just displaying multiple streams at once, but of gracefully handling changes in stream presence and position, user focus, viewport size and shape, and other considerations, without breaking the user's immersion.  The multiview must be a space that preserves itself as much as possible without user direction, intervention, or even notice.

Later, we'll be building some extreme capabilities on top of that foundation, but in this section let's just look at the foundation.

Our first requirement is to display more than one livestream simultaneously in a coherent structured layout.  This will require something like a grid of panels, although "grid" here could included tiled or mosaic layouts where individual panels vary in size and/or aspect ratio, and might even include overlapping panels.  In my implementation, I don't support any of those variants; each panel in my grid is indeed 16:9 aspect ratio and identically sized.  But no matter how much individual panels vary - dramatically as in a mosaic, no variance at all as in my grid, or any other approach - there must be some possible structured layout because positioning is essential for later purposes; we have to be able to recognize "open spaces" and "positioned spaces", and we have to understand the relationship between spaces/positions, in order to place streams dynamically according to user preference and other factors.  And so it's not enough to show multiple streams wherever the user drags them to, because much of the system must behave automatically, and that requires some structure in the layout.

The panels in this structured layout are where we might show an active, playing, stream.  We might use them for other purposes such as chat panels or preview panels or informational panels, but active, playing, streams, should play within a panel in our structured layout, such that we can dynamically position streams through an understanding of the structured layout.

(It's conceivable that the layout may in fact only be showing one stream, or zero, depending on availability and user settings and other factors, but what matters is what it's technically capable of showing.)

This structured layout of multiple stream players provides the basic foundation of our shared space experience.

Now that we have a structured layout, let's make sure it handles expected changes to player availability, such as a player being added or removed or swapped/repositioned.  This seemed simple when I tried it originally; if players exist within the application's user interface, and you want to remove a player, just remove it from the user interface.

In my implementation using an HTML/CSS front-end driven by React, and showing stream players embedded from Twitch.tv, my confidence lasted about 3 seconds into testing.  The problem was that my approach of removing a player from the user interface created technical issues that led other players to interrupt playback and then resume, a jarring disruption and break in immersion.  Adding players worked... if I added them at the end of the code that contained the other players.  But if I added them in the middle, some kind of reflow was triggered that again interrupted many if not all players.  There was also code in the embedded players themselves that seemed aware of their physical place in the page, or possibly their relative location to other players, and moving any player caused interruptions as the other players reset themselves to the new physical location or relative location to other players or both.

What originally sounded like a trivial task actually took considerable experimentation and testing to solve a number of different problems. One of the solutions involved careful memoization and compartmentalization of React components, and careful separation of stream player properties with other properties, leveraging and tuning React's clever capabilities to ensure minmimum DOM disruption, without creating performance or security problems.  Several other solutions were also employed, such as changing the removal process of streams such that instead of removing them from the DOM, they're instead left in the DOM but have their CSS visibility property updated to hidden, thus ensuring continuity of the physical DOM layout throughout the removal process.

But the biggest breakthrough for ensuring this basic adaptiveness in my implementation came from using the CSS order property rather than physical DOM manipulation to position stream panels.  This meant that stream location in the DOM is independent of its location in the UI, which allows me to solve UI positioning problems separately from player disruption problems.

To illustrate how that works, consider that when I add a stream to the grid, I don't add it to the DOM in a position that correlates to where it appears on screen.  Instead, I append it as the last child to the common parent of all the other streams, so that its physical location in the DOM is last, while its on-screen position is rarely last, and instead dictated by its order property.  And moving a stream in the UI is achieved exclusively by changing its order property, again without moving its physical location in the DOM.

These are React- and web-specific implementation details, how I solved the problem in my specific situation.  Other implementations may vary considerably in how they address the potential problem or even whether it arises at all.

But no matter what the platform or technologies, the point remains: it is absolutely crucial that player continuity can be ensured to some significant degree, in order to preserve the space the user is in, and thus their immersion, during basic stream manipulation operations.  There may be no way to guarantee total continuity, but some degree of it should be ensured.

And no matter what, this solution absolutely must enable streams to be added, removed, or repositioned, without a total rebuild of the UI or other major performance problems.  Any solution that cannot offer that basic capability, will not work for our needs, because even the slightest automatic adjustment of stream positions would break the user's immersion or even cause deeper technical problems.

Okay, so now that we've ensured that people (streams) can safely move around the space without the building collapsing and being rebuilt, or causing every other person in the building to trip and fall and have to pick themselves back up, let's consider what other fundamental capabilities our space needs.

In a real shared space, people can walk closer to other people, such as for a focused conversation, or they might move further away in order to experience more of the room simultaneously, to get a broader picture of who's there and what they're doing.

The ability to do this with individual streams seems crucial: a way to fullscreen or at least zoom significantly in one stream, even if only by clicking it to open it in a new window or such.  Some mechanism must allow the user to focus exclusively on one stream.

But it quickly becomes apparent that an individual solution isn't enough.

With as many as 8 or more streams on screen simultaneously, giving the user the ability to focus on one of them denies them the ability to choose groups of streams to focus on.

So what's really needed is also a broader zoom capability that lets the user focus on more than one stream but less than the total possible number of streams, playing or not.

In fact, this zeem feature seems like a necessary capability, not just of moving around the space, but of deciding where they want to sit in relation to it; close to a small group or distant where they can take in the entire crowd, or somewhere in the middle.

The most that can be said against the criticality of integrating a zoom feature is that the browser or device's or other surrounding system may already have a zoom capability that suffices to enable it, in which case the application itself doesn't need one.

In Thirdplace, I achieve this using zoom buttons, and what they actually control, technically, is the number of visible columns in the multiview.  Since we use a grid of equally sized stream panels, and the grid is the width of the viewport, the number of columns will dictate how many streams appear on a row, which necessarily dictates their individual width.  So by zooming the interface in or out, the user is indirectly changing stream size and thus "proximity" in our physical analogy.

In keeping with our above constraints of avoiding disruptive changes, this too requires a solution that does not rebuild the entire UI.  Instead, we update a CSS grid column count property, which triggers a repainting but not a rebuild, and thus does not intrinsically break player continuity and force player reloading, although some automatic quality adjustments can occur which will cause momentary interruption as the players adapt to the best resolution for their new size.

Okay, so zoom enables the user to scoot their chair closer or further away from the people in the shared space.

But what if the size of the space itself changes?

In our case, that will happen if the user's viewport changes, if their browser or tab resizes or their application or screen changes, if they rotate their display, if they move the application to a differently sized screen, etc.  In any scenario where the size of the user interface changes, we need to listen for these changes and recalculate and adjust our presentation to both preserve the space as closely as possible to our user's expressed intentions form the prior size, and to adapt the content and positioning of streams as necessary to reflect the new situation.

Critically, we need to do this without, again, rebuilding the entire UI.  It should be as seemless as possible.

In the case of Thirdplace, I achieve this by listening for window.resize events, calling a debounced handler, then recalculating how many columns can fit based on the current size of the first visible panel, and finally triggering a re-evaluation of visible streams and positions based on the change, because for reasons we'll discuss shortly, it's not practical to show live players for all streams, and so the decisions of which streams to show as live players, and where to position them, is extremely complex, and highly dependent on the available viewport space and zoom level.

Thirdplace also implements minimum stream sizes of 300 pixels wide, and a minium zoom level disallowing zooming out so far that streams would get smaller than that minimum width, and a maximum zoom level of 1 column, which would provide the widest possible stream as it would take up nearly the entire width of the viewport.

These are implementation details specific to Thirdplace, but they illustrate the complexity of these problems and the work that went into solving them just to ensure a solid, adaptive, foundation on which to build the rest of the application.

However it's implemented, this system must support different viewports.

Okay, so we’ve now ensured that we have a stable and adaptive space for our user, as they move around the space and as the space itself changes in size and shape.

But let's look outside the space for a moment.

If we're compressing or expanding the space by zooming or resizing the viewport or other mechanisms, that suggests that there is an "outside" the space for it to compress from or expand into.

Our space exists within a broader space.

In my implementation in Thirdplace, I represent this by showing ALL available streams within the UI, as preview thumbnails in a direct continuation of the same structured layout as the active players, each stream preview in its own stream's panel, and each with optional overlays that, when shown, display their title and channel name and tags and other options and details, allowing the user to quickly scan and understand "the crowd outside the coffeeshop".

To keep these previews from overly burdening the user's hardware, I use very specific tactics like infinite scrolling and lazy loading.  And each stream preview supports several operations, the most crucial being that each preview panel allows and in my implementation actively prompts the user to promote it into the active playing space, essentially to invite it into their coffeeshop.

But otherwise, that's all my specific implementation.  I could imagine showing previews listed on a sidebar instead of within the multiview's structured layout itself, for instance.  But even in that scenario, the previews must still be ordered and behave in such a way that it can readily be understood how they might flow into, or be invited into, the active playing space.

Even "preview thumbnails" is an unimportant implementation detail, as quite a few options for displaying potential streams seem obvious at a glance, such as very low framerate videos or gifs or slideshows, or grids composed of multiple preview thumbnails, or some collage displaying both thumbnails and stream information.  A visual component seems crucial, so that the user can glance "outside the space" and see who's waiting outside to come in, and who's available to be invited in, but what exact form that visual component takes is not, so long as it doesn't overly burden the user's system.

The exact ways this is all implemented can vary, but the function cannot, and is clearly particularly crucial to the experience Thirdplace offers: non-playing streams must exist as a clearly contiguous and easily explorable extension of the active playing space, creating a visible, interactive context for the active playing space, and which connects to it directly and dynamically in a way that preserves spatial continuity. This ensures that streams do not simply appear and disappear unpredictably, but instead flow naturally into and out of the user's immediate focus, maintaining the integrity of the experience as a dynamic, living space, within a potentially vast broader context, and directly tied to that context.

Thus, our multiview isn't simply showing a small set of active playing streams.  It is not a coffeeshop alone.

It is showing a small set of active playing streams that are tightly and dynamically connected to a potentially vast context.

It is a coffeeshop... in a city.

How we dynamically populate those spaces, how we control them, and how we make them come alive, become questions of supreme importance, which we will explore throughout this discussion.

Let's start by talking about how we populate our city.



# Section V: The Uniquely Challenging Data Environment of Livestreaming


We’ve established that the multiview exists as a persistent space—streams come and go, but the space itself remains intact. Now we need to address how that space is populated and maintained in real time.

We know we need to understand, analyze, and present streams, which means doing the same with their data.  This data may include channel names, streamer names, stream URL's, metadata like titles and tags and descriptions, category or game information, etc.  Implementations will vary significantly in exactly what information they use to understand, analyze, and present the available streams, but they WILL need information.

But how do we retrieve and handle that information?

This is not a list of search results. It is not a snapshot of a moment in time. This is a continuous, living space, sustained across hours or days, while everything within it constantly shifts and changes. Unlike a traditional media interface, where users request a set of results and browse them statically, this system must dynamically sustain itself around the user, updating seamlessly as streams appear, end, or evolve.

Livestreams are inherently volatile. They begin and end without notice, change titles and tags mid-broadcast, and may even be misreported as online or offline due to API limitations.

That volatility alone would create issues in many applications, but our situation is even worse, because we're trying to use that that volatile data to sustain an experience that must feel stable and continuous.

To do that, we need a continuous, intelligent data pipeline that keeps the multiview and the entire set of stream data accurate, stable, and alive without breaking immersion.

And that's another crucial factor: we're not just concerned about one page of search results.  We can't just look at a slice of the data.

Our system, whether on the client side or the server, needs to look at the entire set of stream data to understand how best to personalize it and drive it toward or away from the user's active playing space.

Given those concerns, our data pipeline must be:

1. Comprehensive, and

2. Relatively continuous

We need the fullest set of data possible, as frequently as possible, even in real-time if possible.

We also have to be very careful with that data.  We're not showing a snapshot of search results on a webpage, we're delivering a constant, sustained, persistent experience, that might last many hours.  Any significant problems in the data WILL compound and create instability that quickly shatters the user experience.

Once we’ve retrieved stream data, we must also verify it, correct inconsistencies, and reconcile anomalies. A common issue is duplication — streams appearing multiple times in received data, requiring detection and resolution to ensure a consistent view. Similarly, if a stream disappears from an update, we cannot immediately assume it has gone offline, particularly if it is still playing for the user.

Really, our best information comes from the actual player experience, for the few streams that are actively playing or that we try to begin playing. API data is informative, but it is not absolute. A missing entry in the latest update might be a delay in reporting rather than an indication that the stream has actually gone offline. Likewise, the presence of a new stream in the data does not guarantee that it is playable. A properly implemented system must treat API data as a powerful signal, but never as fact.

This means that data verification is absolutely crucial. How that verification is performed may vary across implementations, but any system that fails to reconcile and validate its incoming stream data cannot provide the stable, immersive experience our invention requires.

With our comprehensive and relatively continuous data pipeline in place, and a data verification layer between it and the rest of the application, we now have a stable and self-correcting pipeline that can process vast amounts of streaming data.

But how do we ensure that this data flow doesn't disrupt the multiview experience or overwhelm the user?

We now face a new challenge: how do we ensure performance, continuity, and spatial coherence in an environment where stream data is changing and thus streams are constantly shifting in and out of view?



# Section VI: Preserving Continuity & Performance


We’ve established how our system gathers, verifies, and processes streaming data at scale. But even with perfect data, a new challenge emerges: How do we ensure that streams are presented smoothly, performantly, and without breaking the user’s sense of continuity and immersion?

A naive solution might play whatever streams happen to be in view as the user scrolls around or as a feed pushes them through the viewport. But this would turn the experience into a chaotic, kaleidoscopic experience — an endlessly changing experience ideal for short form content but utterly at odds with the nature of livestreaming, and incapable of providing the sculpted, persistent space that we yearn for.

Instead, our system must ensure that streams within the user’s active playing area remain persistent, regardless of where they browse next. This prevents the experience from feeling like a disjointed reel of clips and instead preserves a stable, personalized space.

To achieve this, the system must ensure three constant goals:

1. Streams that enter the active playing area should begin playing automatically

2. Streams that are in the active playing area should continue playing regardless of other user activity

3. Streams not in the active playing area, or removed from it, should not play except in very specific cases.

This requires defining an active playing area — the portion of the system where streams are actively playing. While a common implementation might use a grid where only streams above the fold are considered active, this concept must remain flexible. Some implementations may use a circular layout, a layered approach, or even a dynamic viewport-based approach, but the key requirement remains the same: streams in the designated active space persist in playback, while others transition into a preview state.

Beyond playback persistence, the system must also provide a way for the user to explore additional streams without losing context. This is not a traditional search or discovery system — it is a living environment, and users must be able to move fluidly within it. Whether through scrolling, a dynamically replacing queue, or another approach, the key requirement is that users can browse beyond their current space without disrupting what they’ve already established.

Since this area is not the active playing area, as the user browses it they might no longer see the active playing area, but ideally the players in that area should continue playing, to avoid disruptions and audio interrupts.  Their quality might be reduced, but the space should remain alive whether the user is inside it or wandering outside temporarily.

Audio plays a crucial role in maintaining immersion without overwhelming the user.  Too many simultaneous audio sources from playing streams would create audio chaos, while too few would leave users without a sense of presence.

I struggled with this originally, and the first iteration of the audio system was overwhelming, not because it lacked the necessary controls but because I didn't understand how to use them.  I was confronted with 8 simultaneous streams playing their audio full volume, and obviously I couldn't distinguish any specific sounds or sources.

In reflecting on this, I thought about our spatial design and how real world spaces manage this problem.  How is it that we can sit in a stadium and have a conversation with someone sitting next to us, despite 8,000 other people in the same stadium also talking?  The answer was that volume attenuates over distance.  So the conversation next to us seems much louder than the conversations further away.

I realized that the right way to think about audio in this dynamic shared space was to treat it spatially; by ensuring that the system offers a way to treat audio from some streams as foreground, and audio from other streams as background.

This solution must enable that level of audio complexity.  It can do so automatically, manually, or both, but it must ensure that focused streams remain clear while others remain ambient but unobtrusive, or muted altogether.

In Thirdplace, we provide global and stream-specific volume controls, encouraging the user to keep the global volume low and using that setting as the default when new streams start playing.

To enhance the background effect of the global volume in my own implementation, I use a simple math trick to widen lower-volume settings on the global volume slider and narrow higher-volume settings:

```
const exponent = 1.52;
const adjustedVolume = Math.pow(value, exponent);
```

That specific code means that a slider setting of, for instance, 0.8, translates to only 0.71 actual volume, slightly lower than the slider would suggest.  Meanwhile a lower setting of 0.2 translates to a mere 0.086, less than half of what the slider would suggest.

That specific trick isn't crucial at all, but helps illustrate how crucial the audio layering itself is; the application must allow some streams to be louder than others, and to set or otherwise determine a default volume (including possibly 0; muted) for new streams that considers the specific needs of our space.

By the same token, stream players should unmute themselves automatically when the global volume is unmuted and they begin playing.  I found with Thirdplace that autounmute does work with the right settings, so long as the user has interacted with a volume control on the page already.  To ensure this, when the page loads, I leave all streams muted until at least one has started playing, at which point I use a spotlight effect to encourage the user to click the global unmute button, which counts as interaction, and thus both unmutes the players and also unlocks future autounmuting by the application.  iOS works differently and never allows autounmute, so on that OS the unmute button becomes a partial-unmute button when new players come into view, allowing the user to unmute them without having to mute other players first, or at the same time.

These implementations are again optional, but they illustrate the extreme focus that audio requires for our active playing area to achieve its goal.  There must be a way to layer audio that creates an effect of foreground vs background, otherwise the solution would be overwhelming when more than one or two streams are playing audio.

Non-playing streams normally don't factor into our concerns of keeping the active playing area continuous and immersive, because, of course, they're not playing at all.  But it's conceivable that an implementation might add a preview system of some kind to watch and/or listen to streams outside the active playing area, which would in fact create some complexity, requiring decisions about how to balance that preview system with the active playing area's needs.  I can imagine an implementation that not only allows previewing non-playing streams but also attenuates the audio from the active playing area while doing so, to better hear the previewed stream(s).  But those are just possible approaches to expand the system; all that's strictly necessary is that the active playing area remain continuous and immersive as much as possible.

Speaking of immersion in the active playing area, to make it truly feel like a social shared space the user is inside and participating within, rather than a spectator, there should be interaction capabilities with the streams.  This will depend heavily on the exact source of the streams and what interaction capabilities they offer to begin with, but our multiview must enable some form of interaction with them.  This could be as simple as the ability to follow links to pages of or related to the streams, it could be the ability to follow/unfollow streams, or subscribe/unsubscribe, or to donate, or any other options.

Interaction could also be in the form of chat.  Thirdplace has a very sophisticated chat integration system that enables the user to open chat panels adjacent to each playing stream, and these chat panels are carefully managed within such that they remain adjacent no matter how the layout or positioning changes.  This adjacency was a careful choice because, if chat is offered at all, for multiple streams, then there must be some way to map individual chat UI's (or individual chat rows in some aggregate solution) to their corresponding streams, as each stream generally functions as its own chatroom.

But not all streaming services offer stream chat, so it's not a necessary feature.  Some interaction capability clearly is, however, otherwise we're not creating a participatory shared space but rather a passive monitoring tool.

Finally, performance constraints must be actively managed to keep the system running smoothly across various devices and bandwidth conditions. Playing too many streams at once would quickly overwhelm even high-end systems, and relying on individual stream players to automatically set their own quality can result in a sort of endless battle royale as they compete to dominate the available resources on the system.  So our solution must consider playback quality, whether automatically or manually or both.  It's imperative that we not, for instance, force countless 4K streams on the user simultaneously when their hardware and bandwidth cannot support that load.  Dynamic quality management, default quality settings, individual stream quality settings, resource monitoring, careful setting and possibly adjustments to the number of simultaneous active players, and other tricks, might all be employed to this end.  It's easy to imagine variations of this where certain player positions have a higher default quality or such, or possibly saving quality settings for individual streams so that they're always given that quality when they come into view.

In my implementation, Thirdplace uses a quality threshold array to assign a pre-set quality setting based on player width.  Since streams vary in exactly which resolutions they offer from our current source, I choose the smallest available quality that's at or higher than the threshold for the current width, to ensure its quality is not too low.  I also adjust quality when a stream is set to fullscreen, changing that stream's quality to auto and every other stream's quality to the lowest available quality since they're behind the fullscreen stream.  My roadmap also includes a user setting for a low-quality mode.

Similarly, non-playing streams must also be carefully managed to avoid overwhelming the system. Even though users may browse thousands of potential streams, the system probably can't fully preload thousands of streams and maintain them continuously without harming performance.  Instead, previews should use approaches like lazy-load, infinite scrolling, and careful cleanup and removal as data changes, to ensure that performance remains stable without sacrificing access to content.

Likewise, when a playing stream is removed from the active playing area or otherwise stops playing, we have to be careful to fully clean it up without disrupting the spatial structure of the interface, avoiding situations where we accumulate unused video players that quickly destabilize the system.

Implementations of performance constraints and considerations for playing and non-playing streams could vary widely, and might even be the default with some approaches, but clearly some resource and performance considerations for both playing and non-playing streams are crucial.

With these strategies in place, the system maintains a continuous, high-performance environment, where the user’s personalized space remains intact even as they explore, while automation helps manage performance without breaking the feeling of immersion.

But even with perfect continuity, we now face another challenge: How do we decide which streams belong in the user’s space?



# Section VII: Sorting & Filtering Engine


Okay.  We built the coffeeshop, we built the city around it, and we invited a massive population to take up residence within that city.  But nobody walks around, nobody moves around.  So far they're just stuck wherever they arrived.

We need to bring the city to life.

Sorting and dynamically filtering is what enables this entire system to make 10 streams, or 10,000 streams, feel vibrant, personalized, structured, and manageable, at all times, and without breaking the user's immersion.

Typical streaming services and other systems operate on a "search -> result" system which is similar to HTTP's request -> response architecture and often built exactly that way.  You want to see content like X so you search X and are shown results in the order they match X.

But that model completely collapses when applied to live, dynamic, and unpredictable content. Search works when results are static, persistent, and addressable, like a movie library or a shopping catalog. But livestreams are chaotic, ephemeral, non-descriptive, and constantly shifting — a great stream now might not exist five minutes from now, and if it does, it might look very different and sound very different and show something very different, and its metadata and self-descriptions are often completely worthless.  Worse, if a stream you'd love starts ten seconds after your search, you'll miss out on it completely.

And the best livestreaming content for you, often isn't something you'd think to search for in the first place.

Instead of surfacing relevant content as it emerges, that old paradigm would hide it behind an endless, blindfolded, guessing game.

For a system designed to deliver a seamless, immersive, and ambient experience, search isn’t just ineffective — it’s irrelevant.

Alright, so we need a different paradigm.

A common approach at this point is the algorithmic feed concept which many social media sites and other applications use, where you have an endless scroll of content passing by like highway traffic.

But that approach only works with disposable content which you don't mind passing out of view as quickly as it comes in.

But livestreams aren't disposable.  They're not short-form video, they're not tweets, they're not chat messages.

They're long-form, evolving, and emergent; even if one doesn't catch your eye immediately, who knows what the next moment will bring.  You'd like a flow of content, some ability to shuffle through what's relevant to you, but you also want a way to pin some of it, to keep it resident where you can glance at it to evaluate what's going on over time, or to focus on it and enjoy it fully.

Alright, so we can't use a purely static feed because it would lack the vibrant openness we need, it would be a classroom rather than a dorm.

But we also can't use a purely dynamic feed because this is a long-form medium where we don't want content we enjoy to disappear on us.

So it seems we need a new paradigm that combines the two.

Something like a dynamic feed, but with permanence.  Something more like a dynamic space, like a coffeeshop, where patrons enter and leave and move around, but where many stay in place, providing continuity and familiarity.

And here, we're not confined by the laws of physics, so we can shape and sculpt that space uniquely to each observer, or better yet, enable them to sculpt it themselves while automatically filling in the open areas ourselves based on what we know about their preferences.

Streams shouldn't just scroll past you, and you shouldn't have to scroll past them.  You should live among them, and they should shape themselves around you.

This is a complicated and counter-intuitive paradigm for web applications, or software in general.  We generally only see it in gaming and virtual world design, where we actually see dynamic virtual spaces.  But in every case of those, they're built around virtual physics, virtual geometry, where the virtual spaces obey the rules of real world physical spaces.

What if we threw out all of those rules and just made a dynamic space that was truly personalized to the user, where their own sculpting and exploration works in tandem with automatic processes that assist their exploration and also surface and suggest content based on their preferences?

So let me talk about how I did that.  It's surely not the only way, but I think any other implementation has to achieve a similar effect: creating a dynamic space that tracks user preferences, allows them to control or influence those preferences, automatically surfaces content based partly or wholly on those preferences, and still allows the user to assert control over their space to preserve their immersion and maximize their experience.

Alright, so we need to make a dynamic space, and we think a multiview will provide that dynamic space, and we have dynamic data coming in to populate it with.

For a dynamic space to be populated with that stream data, we need to be able to map the stream data to spatial positions.  That is, for any stream in our data that should be present in the space, we need to know where in the space it should be placed.  Otherwise how could it be present in the space?

In my implementation, I refer to positions as slots, and simply treat them numerically, ordered left to right and then top to bottom, so the same order as English writing, but I can easily imagine other positioning systems including 3-dimensional ones.  What is crucial between all of them is that there is a way to map a stream to a position in the space, otherwise, again, how could it appear in the space without a position?  Even a random position is still a position.

Now, determining a spatial position for a stream as described above might sound trivial, but it is not.

It is, in fact, the heart of the entire system.

It is what we yearn for when we think about fond memories of college dorm life, or conventions, or festivals, or favorite coffeeshops or pubs or offices.  Every shared space we love is characterized by how it lives and breathes socially, how it changes over time, with some elements changing vibrantly and dramatically and others remaining static and familiar.

These elements are shaped by passive forces and by active forces, both inside and outside the space.

The passive forces are the natural, vibrant, dynamic forces that lead individuals to roam into, around, and out of the space, at their own discretion.  The forces that attract them to the space, the forces that lead them to move around within the space, and the forces that prompt them leave the space, but all natural and emergent rather than actively dictated.

The active forces are the dictated instructions and commands that select and invite specific individuals to enter the space, to move to specific positions inside the space, to stay in those positions, and to leave upon request.

In a coffeeshop, you might invite someone inside for a conversation, then ask them to sit with you. That’s an active force, applied externally and internally.

You can also imagine the shop adding a sign to its window that invites fans of a particular TV show who might be attending a nearby convention to enter the shop.  That is a passive force that shapes and sculpts the people likely to enter the shop, but not in an active targeted way, the sign isn't choosing exactly who should enter, it's merely applying a passive force that, like magnetism, adjusts who the shop attracts.  And every coffeeshop has areas and lines and other spaces designated for open movement, with the expectation that people in them will move around freely, and within these free spaces the crowd would still reflect who the shop is attracting passively.

So imagine that you invite an artist into a coffeeshop for a conversation, but the coffeeshop is passively advertising a welcome message to attendeeds of the local TV show convention.  You've applied an active force that shaped one area of the space, while the passive force is dominating the other areas of the space.

This is exactly how Thirdplace and Workplace work, because it is exactly how shared spaces work, we just never think about them that way, and I'm not sure anybody's ever thought about software that way.

Let's talk about each of these elements of how we position streams within our multiview; our constructed shared space.  What features do we need to achieve each element, the passive forces and the active forces?

1. **Passive positioning forces**.

    Passive positioning forces are the forces that influence the position of occupants in a shared space without a specific active effort targeted at each one.  The forces might be created through an active effort, like placing a magnet or a sign, but then they operate passively, allowing a vibrant dynamic flow within and through the shared space.

    In our multiview composed of livestreams, it would be chaos to have thousands of candidate livestreams chosen randomly for display in the multiview.

    Instead, we need some mechanism for deciding which streams should get preferential positioning over other streams, without direct user intervention.

    That's fundamentally describing a sorting mechanism, a ranking mechanism for streams, which is partly true here.  I cannot envision an implementation of this system that does not have some sorting mechanism for dynamically positioned streams, even if the sorting mechanism is implicit in the source data, like the recency of the stream starting resulting in the most recent stream appearing first or last in server-provided data to the client side, thus creating an implicit sort of most-recent-first or most-recent-last, or the other way around.

    In Thirdplace, the default sort I chose was by viewer count descending.  Absent any other criteria in a category or page, the stream with the highest viewer_count number in its metadata will be in the first position, the second highest in the second, etc.  Ties are left in their initial order within the source-provided data.

    Viewer count is a very useful criteria because it's the strongest indicator of broad popularity for a stream.

    But it has absolutely no direct relevance to our specific user.

    In fact, no possible system so far described would.

    Without understanding the user's preferences, no system could possibly sort streams passively by relevance to that user.

    And so we see a second requirement emerge.  Beyond a default sorting mechanism (possibly selectable), we also need a way to apply user preferences.  It's even possible that user preference could be known so well that there's no separate sorting layer, but for new users we couldn't possibly know their preferences that well, so clearly there must be at least a default (possibly selectable) sorting mechanism, and also a user-specific sorting mechanism.

    These are the two core elements that provide our passive positioning force.  Default/selectable sorting, and user-specific sorting.

    I said that my implementation currently uses viewer count descending as the default sort, and that's true.

    Now let's talk about the user-specific sort.

    The default sorting layer is critical, but it’s also completely impersonal. It ranks streams in a way that makes sense for a general audience, but not necessarily for an individual user.

    For that, we need a way for the space to shape itself around the individual user’s preferences, working passively, but in exploiting user-specific information.

    This raises quite a few options for implementation, for instance using knowledge gained outside of the application, and/or some automated method that trains itself on user-specific data, behavior, or other information generated within the system, like a machine learning or artificial intelligence solution.  We could even imagine a solution driven partially or fully by user relationships in the system, like a feed that shows you what your friends are watching.

    I'll talk about my implementation, but it's far from the only one possible, or even the best.

    In my experience, social media works best when I can influence what I see in it.  Even the smartest artificial intelligence and machine learning algorithms can only speculate about what I might be looking for or interested in at any given time.

    So the solution I wanted was one that I could directly, manually, influence.  By applying an active force once, to express my preference, but which would create an ongoing passive force that keeps shaping the shared space so that it continuously reflects that preference.

    I don't have much information about stream content, but the data I'm using does contain stream titles and lists of tags for each stream.  These are provided by the streamer and can be (and frequently are) updated while they're streaming, so they're a decent suggestion of what the actual stream content is, although of course only as comprehensive or reliable as the streamer chooses to make them.

    I decided that showing a full list of all tags that appear within the stream data, with a visible count of how many streams have that tag, would be a very useful tool for the user to explore the metadata content of the huge set of data.

    But looking isn't enough.  The goal is to personalize the passive positioning of streams, to determine and apply a user-specific preference for or against specific content.  This could be done with some automatic system that doesn't need user action to activate, but I don't have one in Thirdplace.

    So if looking isn't enough, and if we need user-specific personalization and I don't have an automatic way to do it, then my users need a way to actively express their passive preference.

    What I chose was to let users promote or exclude tags in that full list of tag strings.  Each tag is listed with a way to promote streams containing that tag, or exclude them.

    And our preferences can be multi-faceted, so it can't just be one tag that we support.  We maintain an array of promoted tags, and an array of excluded tags, and these are reflected in the UI with dedicated list areas on the same sidebar as the full tags list.  Promoting a tag adds that tag to the promoted array and moves it to the dedicated UI area for promoted tags.  Excluding works similarly, with the excluded array and the excluded tags section of the UI.

    But we also have stream titles, and experience told me that streamers often mention things in titles that they don't set tags for, for whatever reason.

    And titles are extremely diverse, I can't really show a list of strings found in titles.  Instead, I added a "dynamic filter" textbox so that users can just type in a string and add it to the promoted filters array and UI section, and it will be treated like a promoted tag.

    Again, this is only my implementation, I can imagine many different ways to implement the same crucial goal of applying a user-specific preference to our stream data, some automatic, some manual, and some a mixture of the two.

    Now, the way these are applied mechanically is actually pretty simple, and I think probably unavoidable.

    I use a full text search on titles, and a fixed search on tags, to score each stream in the page's data based on its matches to promoted tags/strings, with more matches increasing that stream's score.  Any matches to excluded tags/strings result in the stream getting flagged for hiding so that it doesn't appear at all.

    Then, in my master dynamic sort, I prioritize streams with higher scores, and only apply the baseline default sort to streams with equal scores.

    So at all times, Thirdplace prioritizes streams that match the user preference most, and then, secondarily, it prioritizes streams based on default/baseline sorts.

    While the implementation details will vary tremendously, including user-defined and fully automatic applications of user preferences, the final result seems inescapably crucial: a system that prioritizes the surfacing of personalized content, filling the dynamic shared space with the most relevant content possible for the user, and then, only when it doesn't know enough to use that criteria alone to decide final positioning between specific streams, making estimated guesses about relevance using baseline/default sorting systems.

    A two-stage passive positioning system that operates in an ongoing fashion, which prioritizes user preferences, and employs a baseline sorting system when user preference alone is not available or not sufficient to determine specific stream positions.

2. **Active positioning forces**.

    Above, I described the passive positioning forces that shape the open areas within our shared space.

    But on their own, even in ideal cases, they can still only speculate about what the user wants.  Without the ability to exercise direct, active, control, over some parts of the space, the user is helpless in a sea of algorithmically selected long form content.

    So we have to give users control, some kind of direct interaction or activity that conclusively determines some specific positioning for one or more specific streams.
    
    We could consider a simple pin mechanism for streams that are playing, essentially stapling their feet to the ground, keeping the stream in place where the algorithm put it.

    But two problems arise with that.  The first is that this still leaves us beholden to the algorithm.  The second is that it doesn't help us find and surface content that the algorithm itself did not surface for us, even knowing our preferences.

    Alright, so pinning is insufficient.  It's part of the solution, but not the entire solution.

    The entire solution must also enable the user to move streams around.
    
    At least from the non-playing area to the playing area, so that they can browse and surface content at their own discretion.  It also seems that they would need a way to move streams out of the playing area, either to the non-playing area, or hidden altogether, or ideally both.

    These seem crucial.

    While we're at it, we can also add the option to move streams around within the shared space.  That seems less crucial but still valuable.

    So, for the active positioning component of our sorting system, we need an ability to lock streams to a position, an ability to promote streams to the playing area from the non-playing area, an ability to remove streams from the playing area, and preferrably but critically, a way to move them within the playing area, and specific control over where to send them to when removing them from the playing area; the non-playing area, a hidden area, or both.

    These are the core methods of the active positioning component of our sorting system - some essential, others highly beneficial.

    Remember that we also have the passive positioning system working around pinned streams, and I'll discuss how these separate systems get merged in just a bit.

    But still focusing on active positioning alone, in Thirdplace and Workplace, I implement the operations described above with movement buttons on each stream's overlay, allowing the user to move streams very explicitly and with precise control, although of course implementations could vary considerably, such as using drag and drop or other approaches to achieve the same effect.

    This has been a difficult system to build because precisely positioning streams is not as easy as it sounds.

    Say you position stream "Runebee" in the second position.  Then, the next day, she's offline, and you position "MissKyliee" in the second position.  Then, the third day, both are offline.

    We're preserving the space, as always, so we remember your preferences, but your preferences seem contradictory.  We need a way to reconcile them.

    So it's not enough to have active positioning, we need a reconciliation mechanism, because livestreams are unpredictable.

    My reconciliation mechanism is to rank preferences by recency and then push competing streams down in position.

    So when both Runebee and MissKyliee are online in the above example, I would position MissKyliee in the second position, and push Runebee to the third position because I expressed the preference for MissKyliee's position more recently.

    This suggests that these user actions might not actually "move" anything.  They might instead store or update the user preference toward a specific stream, which is then applied to the interface to indirectly produce an effect that appears to be direct movement.

    But no matter how it's accomplished, we clearly need a way for the user to actively express a preference for a stream to be locked to a position (maybe not its own), a preference for a stream to be moved to the playing area from the non-playing area, a preference for a stream to be in a different position, a preference for a stream to not appear in the playing area at all, AND some reconciliation method for when these preferences inevitably conflict due to the chaotic nature of livestreams.
	
Alright.  We've now created two separate mechanisms that each provide positioning data for streams.

But how do we put them together?

Our goal was to create a space that feels alive — a dynamic, immersive environment where streams don’t simply appear and disappear like messages in a feed, but have a mixture of static and dynamic elements, a familiar yet also vibrant flow like in a dorm or coffeeshop or clubroom.

Active positioning gives users control over their surroundings, providing that familiarity and stability, while passive positioning keeps the environment fresh and vibrant, seamlessly surfacing new content.

The challenge is to merge these two forces without breaking immersion — so that dynamically suggested streams move fluidly into and through open areas, while user-placed streams remain comfortably anchored.

Okay, so we need some merge feature somewhere in our system that takes into account both factors, the passive positioning information and the active positioning information, and it will usually prioritize active positioning information when available.

There are countless ways to implement this merge feature, and it might take place in separate spots of the subsystem or in a single spot.  It could even happen directly in the presentation layer.  What matters is that it exists at all.

In Thirdplace, the merging system first separates actively-positioned and passively-positioned streams into two separate arrays each sorted by position preference.  Then it creates a new, empty array.  Then it loops through both of the stream arrays sequentially, moving streams into the new, combined, array, as appropriate, based on the position preference.

The pseudocode for this merging loop in Thirdplace is as follows, but remember that this is only one of countless possible implementations with countless possible architectures:

```
const combinedStreamsData = [];
const streamsToAppendAtEnd = [];
while (
	(streamsActivelyPositionedIndex < streamsActivelyPositionedLength)
	|| (streamsPassivelyPositionedIndex < streamsPassivelyPositionedLength)
) {
	if (streamsActivelyPositionedIndex < streamsActivelyPositionedLength) {
		const streamActivelyPositioned = streamsActivelyPositioned[streamsActivelyPositionedIndex];
		if (streamActivelyPositioned.preferredPosition > 8) { // indicating hidden streams
			streamsToAppendAtEnd.push(...streamsActivelyPositioned.splice(streamsActivelyPositionedIndex));
			streamsActivelyPositionedIndex = streamsActivelyPositionedLength;
		} else if(
			(
				combinedStreamsData.length >= 
				Math.min(
					streamActivelyPositioned.preferredPosition,
					maxPlayersCount
				)
			)
			|| (streamsPassivelyPositionedIndex == streamsPassivelyPositionedLength)
		) {
			combinedStreamsData.push(streamActivelyPositioned);
			streamsActivelyPositionedIndex++;
			continue;
		}
	}
	if (streamsPassivelyPositionedIndex < streamsPassivelyPositionedLength) {
		if (
			(streamsActivelyPositionedIndex === streamsActivelyPositionedLength)
		) {
			combinedStreamsData.push(...streamsPassivelyPositioned.current.slice(streamsPassivelyPositionedIndex));
			break;
		} else {
			combinedStreamsData.push(streamsPassivelyPositioned.current[streamsPassivelyPositionedIndex]);
			streamsPassivelyPositionedIndex++;
		}
	}
}
combinedStreamsData.push(...streamsToAppendAtEnd);
```

This loops through both streamsActivelyPositioned, and streamsPassivelyPositioned.  If the current actively positioned stream has been actively positioned to the current position or a higher one, it places that and skips the rest of that iteration's processing.  Otherwise, if there is a passively positioned stream available, it places that.

It continues until every stream in both arrays has been placed, doing some in batches when it makes sense to.

In this way, for every position, actively positioned streams eligible for that position (having been positioned to that position or a higher one) are prioritized over passively positioned streams.

This again is just one of countless ways and architectures to handle the merging, but it should illustrate what merging needs to achieve.

There's also the consideration of the active playing area changing; what happens when it can no longer show all the actively positioned streams?  I haven't found an easy answer for this, some trade-offs are inevitable, and I'm not yet convinced that a solution is even necessary although it might be.  As an example of how to solve it, in Thirdplace I do so with a fast compression sort after any sorting or resizing.  During that fast compression sort, if the actively positioned streams don't fit in the active playing area because it's too small, but otherwise would, then I remove free slots from the active playing area as needed, starting at the lowest to minimize displacement of higher streams, and shift actively positioned streams higher as space becomes available, to try to fit them into the active playing area.  This is a complex implementation but it provides a more intuitive sense of control and as much stability as I can, while still prioritizing active positioning over passive positioning.

So merging is complex and tends to create challenges that in some cases may not have any easy answers.

But it's worth it.

By merging passively positioned streams and actively positioned streams in a manner that favors active positioning, we create the effect of a true shared space - interspersing vibrant, dynamic elements with comfortable, controlled ones.  This dual system ensures that user-placed streams act as stable "anchors" within the space, while passively positioned streams dynamically adapt to fill remaining open areas, surfacing new and relevant content without disrupting the user's sculpted environment.  It produces a continuously vibrant yet stable environment — one that behaves like a real shared space, blending comfort and discovery.


# Section VIII: Workplace & Enterprise Extensions


Okay, so far we've been talking about what we currently call Thirdplace, an application that transforms public livestreams into a massive, personalized, shared space.

But what if we could adapt the same technology to deliver private shared spaces using private livestreams?  Something like a private, virtual, open office?

Physical open offices provide ambient presence and visibility; a subtle awareness of colleagues working around you, even when you're not actively engaging with them, and the motivation and productivity that comes from being visible yourself. These spaces foster mutual understanding, collaboration, spontaneous interactions, and a sense of shared momentum, and that’s all extraordinarily difficult to replicate in remote work.

Traditional remote work solutions - video meetings, team chat apps, project management tools — are great for structured or scheduled communication but fail to recreate that background presence.  You can call a meeting, send a message, or schedule a one-on-one, but there's no way to just "be around" your team the way you would be in an office.  No informal glances across desks.  No passive sense of who's deep in work or what they're working on or why.

Remote coworkers are invisible to one another except during scheduled meetings or as icons in team software.  When they leave a meeting, they vanish.

This is such a glaring, massive, and hopeless, problem, that people have given up even talking about it.  The world takes it for granted, and the only discussions about remote work aren't how to fix it, but whether to bother with it at all.

I don't accept that.

I believe it's a solvable problem, using the same ambient spatial technology that drives Thirdplace, albeit with some appropriate twists.

I call this solution "Workplace", differentiating it from "Thirdplace", and in keeping with our theme of closely following (and arguably improving on) real-world models.

But Workplace can't just be an application.

Thirdplace is an application because the source of the streams or how they're transmitted to its users doesn't particularly matter to its functionality.  In fact, it could comfortably aggregate many different sources of public streams without any real issues beyond scaling up.  It currently runs against Twitch.tv streams, but literally nothing in the application prevents it from also incorporating Youtube livestreams, Tiktok livestreams, Twitter/X livestreams, etc., and not just as separate applications but aggregated into a single unified presentation, because why not?  

Thirdplace is designed as a massive public space.

Workplace is not.  Workplace is the opposite.

Workplace is designed as a private, virtual, open office.  And just like real offices, that means a small, access-controlled, secure, environment, full of confidential information, but where team members share ambient visibility, not just of themselves, but of what they're working on, to the extent they feel comfortable sharing it.  They can glance over and see what their teammates are up to, ask them questions, suggest changes, or generally just benefit from that mutual visibility and ambient presence.

This is such a powerful force that even individuals seek it out, in coworking spaces, in coffeeshops, everywhere they can.

In fact, we've once again found ourselves in the coffeeshop analogy, and that's not a coincidence.  Rather, that's the core of Thirdplace and Workplace; a virtual solution for persistent, ambient, shared spaces.

Okay, but back to Workplace.

To better understand Workplace, let's extend our open office metaphor a little bit.

In a physical open office, team members can generally see what their teammates are working on.  Obviously this requires consent and choice, we're not talking about employee monitoring but simply ambient presence and consensual visibility, as in a coworking space.

Typical virtual work solutions focus, at best, on showing ambient presence of "the worker", but never "the work".  They may show little cartoon figures or images or sometimes even webcams of the team members to each other, maybe in little rooms on a screen or as icons on a diagram or whatever else.  But that's not what we want.

What we want, is to see the work.  Or beyond that, what we want is to see the tuned, sculpted, presence, of the team member.  Their sculpted stream, their space.  Within the broader space.  Maybe their presence is their integrated development environment, surrounded by a personalized border image of a starship bridge, with an inset webcam showing their cat laying on a chair.  Maybe it's a complex deployment server that constantly shows the state of active IT deployments, a common screen that every team member benefits from having ambient visibility of in and around their colleagues' streams even if it's not technically "a team member".  Whatever the presence is, it can be as informative, as sculpted, as frequently adjusted, and as personalized, as any other livestream.  And we'll call all the stream sources "team members" for simplicity, because in a sense, they are all occupants of our team space.  (Which may not even technically be "a team", but again, let's call it that for simplicity.)

So these presences must be livestreams, and they must originate from the team members' devices.  And Thirdplace's technology gives each team members (or authorized user) a revolutionary way to perceive those streams, to view and engage with them in an virtual, ambient, shared space.

That all sounds very straightforward.

But also abjectly horrifying.

Can you imagine a team of workers on a confidential project livestreaming their work publicly through Twitch?

We need to unpack the implications of our simple goal here, of enabling team members to continuously stream their work to one another.

Let's try to follow this system through to its natural conclusions and develop a solution that turns the horrifying into the mundane, the impossible into the every day.

Clearly, one immediate issue is that the livestreams cannot be shared publicly.  They're confidential.

This doesn't just mean that they cannot end up in a public location, but that the content within them cannot even be transmitted publicly in any readable fashion.

This means that our system MUST incorporate a completely secure architecture that extends from the individual user devices through to the presentation application back on those devices.

And that security must start the moment the stream leaves the user's machine.

There are two fundamental ways to ensure that no unauthorized party can intercept or view these streams in transit. Either:

1. The stream data itself must be encrypted before it leaves the user’s device, or

2. The entire transmission must occur within an encrypted tunnel of some kind

So long as one of these options is used, stream security should be guaranteed, and the confidentiality of the work streamed should be protected.

But then what do we do with these streams?

If our goal is provide each user with am ambient persistent space composed of multiple livestreams from their coworkers (and likely their own as well), then the simplest approach, in theory, would be for each end user to automatically transmit their stream signals directly to each other authorized team member, some kind of peer-to-peer approach.

But that theory collapses almost immediately under real-world constraints.

For a fullscreen livestream to be readable on a high definition display, a stream quality of 1080p and a framerate of 30fps are recommended.  Less, and the stream can appear blurry or choppy or both.  That level of quality requires a minimum data transfer bitrate of around 4.5 Megabits per second (Mbps).

If a user has 9 teammates in their virtual open office, and for some reason all the teammates are watching their particular stream at fullscreen, that would require 9 outbound streams of 4.5 Mbps each, for a total of over 40 Mbps nominal.

Average residential outbound bandwidth in the United States is currently around 20 Mbps, barely half of the average we would require for that scenario even without accounting for spikes and troughs in the streams.

And that's on top of whatever other bandwidth the streaming user and their household are using for work or other productivity or entertainment or whatever else.

Some trickery could be done here with relaying the stream signal to distribute the outbound bandwidth between some of the team members, but that would incur significant latency and still not fully eliminate the problem.

Clearly a peer-to-peer approach won't work for our needs.

That means we need one or more servers to distribute the streams.

But is it even that simple?

No.

Let's imagine that our server infrastructure receives and immediately sends all streams to each user at full quality.  With a team of 10, that means each recipient might be receiving 45 Mbps downstream.  That's actually within average residential bandwidth of 100-200 Mbps, so that's doable.

But 10 full size video streams playing continuously will require substantial user hardware to run comfortably, particularly since those users will likely be doing actual work while these streams are available to them, and thus using their systems for other purposes that take priority.

One option to resolve this is to limit the number of playing streams, and Thirdplace's design gives us ample tools to give users visibility over non-playing streams, but those systems rely on some server processing of the non-playing streams to generate, update, and provide preview images, gifs, or low framerate videos.

The preferred way to solve this would be to transcode the stream signals into lower quality versions and only provide the necessary quality versions for the player size on each recipient user's machine.  So if they're seeing 9 panels in their virtual office active playing area, which easily divides into a fullscreen view at the same aspect ratio, we could reduce the quality of the streams in each player to maybe 480p or less, conserving recipient resources without degrading the experience.

But that would take significant work on the recipient end, which returns us to the same resource utilization problem.

So the transcoding step has to happen upstream.

It could theoretically happen as simulcasting on the sending end, where the user's streaming software encodes multiple qualities and sends the stream signals to the server(s).  This would require more work on each user's device, which we would rather not require, but it actually seems like a viable implementation of this step in the system.

A better implementation would transcode on the server(s), which would minimize resource consumption on each user's device.

This creates a new problem in that transcoding software needs to read the stream data, which means it needs to decrypt the stream data if it's encrypted, or have access to the stream data if it's transmitted through an encrypted tunnel.

Either way, the transcoding software, and whoever manages it, will have direct access to the unencrypted stream data of each user.

Since that stream data is confidential, that means that the transcoding software has to be entirely managed by the team and/or by parties authorized by the team, and it must re-encrypt the streams before sending them along to end users.

This transcoding might also happen on the sending end instead, which would simplify the system by allowing the fully encrypted streams to be sent to one or more servers outside the team and then distributed back to team members without ever being decrypted in transit, though it would use more resources on the sending machines.

Therefore the two possible stream server options for Workplace are stream servers that have trusted access to decrypt and transcode the stream data before re-encrypting it and passing it on to end users, or transcoding on the stream origin devices into potentially untrusted stream servers which won't have to decrypt the stream data before passing it on to end users.

(This could all utilize a single stream server for the Workplace installation, or even across installations, but let's use the plural "stream servers" for simplicity.  And none of it rules out additional servers such as for relaying.)

As far as server configuration and streaming protocols, several different protocols are available, so the exact protocol choice doesn't particularly matter, although RTMPS inbound from end-user streaming software to the server seems simple and preferred at the moment, while WebRTC outbound from the server to the client application is probably preferred at the moment over other options like LL-HLS due to greater compatibility although it probably requires an SFU on the server.  Options abound and the best technical implementation will certainly change over time.

In any event, whichever protocol and server is selected, and wherever the transcoding happens, and thus whether the stream servers have to be trusted or not, let's look at the next challenge.

Once the stream servers have received and transcoded streams, how does each client know which streams?  Unlike traditional streaming platforms, where users manually select a single stream to watch, Workplace must manage multiple simultaneous streams while ensuring that only the necessary data is transmitted.

This will certainly require a stream metadata distribution system, where clients receive metadata that enables them to begin playing streams.

But how exactly should we do that?

Let's think through this very carefully, because Workplace is designed for teams where we expect a relatively small number of streams, which provides considerable flexibility to implementing that particular sub-system.

In fact, due to the small number of streams, it's reasonable to assume that Thirdplace's preview system and extremely powerful metadata sorting and filtering systems probably are not required in Workplace, although they'd certainly be advantageous.

Instead, in Workplace, it's possible that all Workplace front-ends could easily show all available streams at all times, with only adjustments to the quality of the streams to conserve resources, making filtering and preview systems largely unnecessary.  (Although, again, advantageous.)

(Please note that if transcoding is skipped, then some or all aspects of Thirdplace's sorting and preview systems will probably be necessary in Workplace because even a small number of full quality streams could easily overload clients without dynamic sorting and preview solutions like the ones built into Thirdplace.  Workplace is a complex solution with several possible implementations, each of which has tradeoffs.)

But back to our stream metadata distribution system.

Several possible implementation methods occur to me, and others might also be possible.

1. As in Thirdplace, the server(s) may periodically push metadata updates to all connected clients.

2. With its higher trust environment, Workplace clients could be trusted to periodically request metadata updates from the server(s), pulling updates rather than waiting for them to be pushed.

3. A direct peer-to-peer system could be used to bypass the server(s) entirely for the purpose of stream metadata updates, pushing or pulling them directly to or from other clients.

I prefer Thirdplace's system where updates are pushed from the server, which obviates any concerns about trust or client-side debugging or such, and avoids the complexity of creating a peer-to-peer solution.

But regardless of the exact implementation, the stream metadata distribution sub-system must ensure that:

1. Only the stream data necessary for streams actively displayed and playing on the client are delivered to the client, as opposed to delivering unused data and wasting resources.

2. Stream quality is appropriate to the size of the stream player on the client.

3. Stream quality adjusts dynamically as player size changes.

4. Stream availability metadata is updated in an ongoing fashion to reflect which streams are available, ensuring that new streams appear as available in the clients, and ended streams appear as unavailable if they appear at all.

These requirements are necessary to ensure that individual users do not have their resources wasted or their focus or immersion broken by incorrect stream qualities, misleading online/offline statuses, missing online streams, or a need to manually adjust quality or other settings.

Alright, so we’ve gotten Workplace to the point where streams exist, are distributed, and are dynamically managed based on the user’s viewport and bandwidth constraints.

But that’s just logistics — it’s about making sure the system works smoothly.

What we haven’t answered yet is who actually gets to see what?

In Thirdplace, that’s not a concern. Thirdplace uses public streams.  You show up, the system helps you find streams, you watch.  There are no barriers because the whole premise is discovery.  But in Workplace, it’s the opposite.  These streams are private and confidential.

So how do we control who should have access to them, and who can even transmit them into the system?

These are critical questions.

Clearly we can't just let anyone stream into the solution or watch streams shared within the solution, so an authentication solution is necessary.

We also can't just let users authorize their own access, because that's the same as having no authentication system at all, and so our authentication solution needs to be centrally controlled.

This solution will verify user authorization to stream into Workplace, and user authorization to watch streams shared through Workplace, although not every user necessarily has both permissions, and the authorization of either permission may be very granular, like only having access to see some specific streams within the workplace, or only streams of specific teams within the workplace.  It might also restrict or control access to various other features within the Workplace, such as the ability to sort streams or to mute or unmute them for all team members, such as to mute a particular stream to every user if, for instance, some technical feedback loop causes audio problems, or in the event that some confidential or otherwise private information is accidentally being shared.

This is getting complex, so let's describe it in a technically precise manner:

Workplace requires an authoritative authentication solution that verifies user authorization to stream into the Workplace, and verifies user authorization to watch streams, whether in a global sense of having access to all streams available in the installation, or in a more granular sense of deciding which streams they have access to.  Within that solution, access control could be even more granular, allowing varying access to different streams or features within the Workplace, or only access to transmit but not watch streams or vice versa, but it must at a minimum support the above.

Obviously there are countless ways to implement a solution described that way, including integration with enterprise identity management systems, but any implementation must satisfy those requirements, and it seems that a central identity management solution residing on the same server as the stream server is the simplest and most obvious possible implementation, reducing system complexity and simplifying management.

I also recommend, as a best practice, that all team members who can stream into the solution also have access to see streams shared within the solution, and that non-streaming users with access to see streams be kept to a minimum to avoid creating concerns about this being an uncomfortable employee monitoring solution designed to punish unproductivity, rather than a team coworking solution designed to enhance productivity.

Regardless, we now have an authoritative authentication solution in place, but we haven't looked at how the front-end talks to it.

Let's talk about the front-end altogether.

While Thirdplace is designed to present a coffeeshop or dorm experience with a much larger virtual city, Workplace is designed to present a small virtual open office.  And while offices are often located inside larger buildings, just as teams often exist inside larger companies, Workplace remains primarily focused on the team experience.

The team experience of a physical open office is one where teammates work visibly near one another in a shared space, able to motivate and support one another and to feel motivated and supported.

This shared space requirement means that, by and large, Workplace demands the same technical capabilities as Thirdplace.

However, Workplace's front-end differs from Thirdplace's due its much smaller scale and unique security environment, just as an office differs from a coffeeshop.

Unlike a coffeeshop, an office obviously is not open to the public.  Even during business hours it has locks on its doors.  And people who work there have a way to enter it, keys or cards or something.

We've already described Workplace's authoritative authentication system, which serves as the locks on the door, but we haven't yet given its users any keys for those locks.

So we'll have to give users a way to authenticate themselves from the client side.

This would presumably be a login form, but it might also be a single sign on solution of some form, possibly integration with a corporate network environment that their system automatically logs into.  It's possible that authentication into a VPN grants sufficient access to also access the Workplace installation served through that VPN, and possibly to identify individual users.

Whatever the exact implementation, and the simplest and most obvious is a secure login form, Workplace's front-end must have a way for the user to authenticate themselves to the authoritatively controlled authentication solution.

But the authentication is also needed on the streaming side.  The nature of Workplace is that users are likely to be both streamers and viewers; streaming their sculpted workspace into the solution, and viewing the sculpted workspaces presented by the solution.

The two ends might conceivably be implemented in the exact same front-end software, thus likely being able to reuse the user's authentication between the ends, both streaming and watching.  But currently I expect that the end-user sides of the solution would be split with streaming using separate software from the Workplace front-end where streams are viewed.  Both pieces of the end-user experience need to be authenticated somehow, whether using some implicit technology or an explicit login form or key or such.

This authentication capability must not just provide access to the Workplace viewing solution, it must also ensure that the streams viewed within that solution are decrypted and readable by the viewing software.

As to viewing those streams, we must consider that Workplace is designed for a significantly different use case than Thirdplace.

[[removed - Thirdplace is designed to handle a potentially massive number of streams, while Workplace might be implemented for a team of only four users, for example.  This changes the requirements for display adaptability as well as even for immersion, since streams going online and offline would be relatively infrequent events.]]

Thirdplace is designed to handle a potentially massive number of streams, while Workplace might be implemented for a team of only four users, for example.

This changes the requirements from Thirdplace in several interesting ways.  One is that Workplace might completely omit Thirdplace's integrated audio and interaction features, since teams could probably rely on external tools like Slack or Discord for communication.  Another is that display adaptability would likely be difference and possibly simpler, since streams going online and offline would be relatively infrequent events, and obviously there's a much fewer number to accommodate than Thirdplace is designed for.

In such small use cases, this could reduce or even obviate the need for Thirdplace's extremely powerful sorting and preview systems. A simple grid display that randomly positions streams might suffice in such an implementation — if, and only if, that system still preserves the shared, spatial, ambient nature of the virtual office.  Therefore, it would also still need to adaptively manage the resolution and/or quality of each stream based on its size and prominence on the screen, communicating with the stream servers to receive the appropriate stream data, and it would still need to give users the ability to focus on any stream, by enlarging or fullscreening it or some similar approach, without breaking the overall integrity of the shared space.

Because even if it's a very small team, they are still inhabiting a shared space, and thus it is still absolutely necessary to dynamically manage that spatial environment in a way that allows the user to engage, focus, and remain immersed, without overly taxing their equipment and network connection.

Whether that dynamic management system includes full dynamic sorting and complex metadata-driven filters as in Thirdplace, or something as simple as the ability to focus on a single stream via fullscreen or enlargement or some similar implementation — the environment must dynamically shape itself to maintain the persistent, ambient, spatial connection that defines Workplace.

Thus, Workplace must retain the adaptive multiview aspects of Thirdplace, with the possible exception of looser autoplay and play interruption restrictions.  But rather than combining them with the powerful sorting and preview systems of Thirdplace, Workplace essentially moves filtering to the authentication layer, and previewing to the quality management system.  Instead of Workplace's front-end deciding what streams should be shown in the active playing area, Workplace's authoritative authentication system decides that.  And instead of Workplace's front-end having an area outside the active playing area in order to limit hardware use and ensure immersion, it must utilize an adaptive display and quality management system to achieve those goals.  And instead of using a global zoom capability to move around the active playing area, there may be few enough participants at maximum that the ability to zoom in on a single stream via fullscreen or enlargement may suffice.

Nevertheless, we still require the ability to decide what streams are shown in the active playing area, we still require dynamic display and quality systems to ensure immersion and resource management, and we still require the ability to move around the space.

And remember, Workplace is not just a video display system or a streaming platform.  These front-end elements alone are necessary but they're not Workplace.

Workplace is a carefully integrated and interdependent architecture that spans from the user's stream source, through secure transmission and authoritative control, through adaptive distribution and quality management, all the way to our dynamically shaped ambient display environment that preserves the sense of a persistent, shared space.

Each component — stream security, stream distribution, stream metadata and quality management, adaptive display logic, and authentication and authorization control — is necessary to deliver the full solution.  And the full solution is itself the invention.

From first principles and an exploration of our deepest human yearnings, through a fractal of complex technological exploration, we've arrived at an end-to-end architecture that delivers something that science fiction has always promised but which nothing in history has ever delivered: an immersive, ambient, persistent, and totally secure, shared space.


# Section IX: Conclusion


This is just the beginning.

I built Thirdplace because I wanted a persistent, living, shared space, online.  But I can only
imagine where it could go from here. How people might use it, or how it might grow.

Virtual conferences? Tournaments? Clubs?

Or maybe something completely new.  Something that was never possible in the physical world to begin with, or in the 
virtual worlds that people keep creating.  We're certainly not bound by physics or geometry the way that they are.

So the real question isn't "where could this technology go".  The real question is, "what kinds of shared spaces
do we wish we had?"

Because that's the promise of this new technology.  A massive, living, personalized, shared space, far beyond the promises of science fiction, cyberpunk, virtual reality, massively multiplayer gaming, social networks, and more.

My dream is that Thirdplace and Workplace help connect people, in ways that many yearn for without even realizing it.

Technology that truly connects people instead of dividing them.  That lets them feel as if they're sitting in a coffeeshop next to the entire world.

Wouldn't that be wonderful?

- Jeff Richman, April 7, 2025

*© 2025 Jeffrey C. Richman. All rights reserved. No license is granted for use, reproduction, or redistribution of this content without written permission.*




