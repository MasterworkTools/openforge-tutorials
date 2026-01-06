# File Name Standard

Note: curly brackets are not used on the file name format, they are used here to indicate a section.

## Top Level

{texture}#{shape}.{size}.{connections}.stl

## Texture

Texture can be broken up into {wall texture}%{floor texture}.  If a wall texture has only one default floor texture, the floor texture is omitted.

Examples:

`cut-stone`

`dungeon_stone%block`

## Shape

Shape has a basic structure of {shape}+{options}

Both texture and options can have more than one element which is comman separated.  Items in these lists go from more general to more specfic.  The +{options} section is optional.

Examples:

`wall`

`door,arched+wide`

## Size

Size comes in the form of {size}+{options}.  Sizes tend to come in two forms combinations of letters, or numbers in {X}x{Y}, {X}x, x{Y} format.  If it's numbers, {X}x{Y} indicates that the object is X by Y in inches.  Sometimes one of these will have a decimal as in 2x0.5.  Period is also used as the separator with the next area, connection options, so this is only ever the case with numbers, and connection options will never start with a number.  {X}x indicates that said object is X inches long.  x{Y} (fairly rare) indicates that the object is Y inches wide.

The +{options} section is optional, and contains a comma separated list of options to the size.

Examples:

`E`

`2x`

`4x2`

## Connections

This section contains connection systems, and it's format is {connection}+{options}.  Both portions can be comma separated, and are aimed at being from more general to more specific.  +{options} is optional.

Examples:

`openforge`

`openlock+side`

`openforge+side,dragonlock`

# Other Files

There are other files in the heirarchy that are not tiles.  The names cna be more haphazard, but in general I try to have them follow the File Name Standard as much as they can, but in many cases they will wholly skip some sections.

Examples:

`wood#door_lintel+c`

`portcullis+wide,split,a`