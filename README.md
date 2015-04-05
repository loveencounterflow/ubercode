




# ubercode

Extending Unicode Crowdwise


## Foundational Thoughts



>    I get the strong feeling that instead of making all these images part of a
>    standard that used to be all about writing proper (and also because of the
>    inherent openness and cultural issues), i think it would be about time to
>    factor such things out of Unicode proper.
>
>    What i'm thinking of is some sort of extension mechanism that people and
>    organizations can opt-into, using the great software infrastructure that
>    Unicode has caused to exist, but without altering or adding to the standard.
>    That would also be great for a lot of scholarly activity in the realm of old
>    scripts and communities using as-yet unencoded or deficiently encoded
>    scripts. That mechanism could use the Private Use Area codepoints; it would
>    be in need of some modifier codepoints to indicate exactly which
>    interpretation (and which downloadable font resources) are intended to be
>    represented.
>
>    The mechanism could use something akin to interlinear annotation marks to
>    add information to a text what interpretation is intended for subsequent PUA
>    codepoints.
>
>    For example, a text like "foo{http://folk.uib.no/hnooh/mufi/specs/MUFI-
>    Alphabetic-3-0.pdf}bar" (where the curly braces have to be replaced by
>    special codepoints similar to the annotation marks, the URL should not point
>    to a PDF but to a formally defined HTML resource that details intents and
>    downloadable fonts, and the part should be replaced by a suitable
>    representation of that codepoint) could indicate that the text to be
>    rendered should be "foobar" (i.e. seven letters, with the fourth one
>    interpreted according to the Medieval Unicode Font Initiative's proposal). I
>    know this does look awkward, I know this is just off of the top of my head,
>    I know this goes way beyond encoding text as we know it and starts to look
>    like markup, I know there's a danger that URLs just vanish and then you
>    can't reconstruct the text. I'm also aware that if you don't put the URL in
>    front of every single PUA character, chances are such an annotation that is
>    found near the start of a text is likely not to get copied over when someone
>    selects a line near the end of a text. But then something similar is bound
>    to happen all the time when people copy text from the middle of a text or
>    HTML document—a lot of contextual information gets jettisoned.
>
>    But consider: Unicode does provide Private Use codepoints, but does not
>    provide a universally agreed-on way to share those codepoints. If it did,
>    the standard could be freed from a lot of pressure to implement this,
>    implement that, and we still could have a global, unified encoding scheme.
>    Also, we could in fact annotate our PUA usages in a more consistent and more
>    future-proof way.—Sunday, April 05, 2015 3:14:00 pm

>    Just two more things to complete the above proposal:
>
>    We probably need one way to annotate plain text and another to annotate
>    HTML; at least it looks like one should take advantage of the annotational
>    nature that new HTML tags offer (i.e. they get ignored by those User Agents
>    that haven't implemented them).
>
>    Second, the Unicode consortium could curate a list of approved
>    URL/interpretation pairs. This could help to partition the space of the
>    encoding into several spheres or grades: A—the current Unicode standard;
>    B—PUA extensions endorsed and listed by Unicode.org (NB conflicting usages
>    of single codepoints must be possible, that's what the disambiguating URL is
>    for); C–any annotated PUA usages that are not officially listed; D—any
>    unannotated usages of PUA codepoints.—Sunday, April 05, 2015 3:21:00 pm
