# fetch_emojis Discord Bot
### by riggedCoinflip

## raw Command Below

This Bot uses the Guild.emojis as described in:
https://discordpy.readthedocs.io/en/latest/api.html#guild.emojis <br>
to create a JSON-File containing these keywords as:
<blockquote>
    { <br>
    &emsp;    "emoji.name" = "str(emoji)",  <br>
    &emsp;    . <br>
    &emsp;    . <br>
    &emsp;    . <br>
    } <br>
</blockquote>

with str(emoji) containing name and id.

for example:
<blockquote>
    { <br>
    &emsp;    "foo" = "&lt:foo:123456789012345678&gt", <br>
    &emsp;    "bar" = "&lt:bar:987654321098765432&gt", <br>
    &emsp;    "ack" = "&lt:ack:2582012840158349683&gt", <br>
    &emsp;    "wibble" = "&lt:wibble:287394871261947134&gt" <br>
    } <br>
</blockquote>

Attention: This overwrites a (probably) existing file in path.

To use the Bot, follow the instructions on https://discordpy.readthedocs.io/en/latest/discord.html
and replace Token in the last line (bot.run('Token')) with your generated Token.

Change the Path Variable to where you want your File saved.
Then write !emojis_json in your Server to fetch the emotes.
