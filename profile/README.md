# Games

<script>
async function download() {
    const params = new URLSearchParams(location.search);
    const game = params.get("game");
    const platform = params.get("platform");

    const response = await fetch(
        `https://api.github.com/repos/dinamika-games/${game}/releases/latest`
    );

    const release = await response.json();
    const asset = release.assets.find(
        asset => asset.name.toLowerCase().includes(platform)
    );

    if (asset) {
        location.replace(asset.browser_download_url);
    } else {
        document.body.textContent = "Download not available.";
    }
}

download().catch(() => {
    document.body.textContent = "Could not retrieve the latest release.";
});
</script>

All games are free and open source.
No Internet connection whatsoever is used.

Download the latest version for your operating system:

- **Auslender** — [Windows](https://dinamika-games.github.io/download.html?game=auslender&platform=windows) | [macOS](https://dinamika-games.github.io/download.html?game=auslender&platform=macos) | [Linux](https://dinamika-games.github.io/download.html?game=auslender&platform=linux)
- **Bird Dog** — [Windows](https://dinamika-games.github.io/download.html?game=bird-dog&platform=windows) | [macOS](https://dinamika-games.github.io/download.html?game=bird-dog&platform=macos) | [Linux](https://dinamika-games.github.io/download.html?game=bird-dog&platform=linux)
- **Drunken Vikings** — [Windows](https://dinamika-games.github.io/download.html?game=drunken-vikings&platform=windows) | [macOS](https://dinamika-games.github.io/download.html?game=drunken-vikings&platform=macos) | [Linux](https://dinamika-games.github.io/download.html?game=drunken-vikings&platform=linux)
- **Ergo Chaos** — [Windows](https://dinamika-games.github.io/download.html?game=ergo-chaos&platform=windows) | [macOS](https://dinamika-games.github.io/download.html?game=ergo-chaos&platform=macos) | [Linux](https://dinamika-games.github.io/download.html?game=ergo-chaos&platform=linux)
- **Head Invaders** — [Windows](https://dinamika-games.github.io/download.html?game=head-invaders&platform=windows) | [macOS](https://dinamika-games.github.io/download.html?game=head-invaders&platform=macos) | [Linux](https://dinamika-games.github.io/download.html?game=head-invaders&platform=linux)
- **Jump 'n' Mine** — [Windows](https://dinamika-games.github.io/download.html?game=jump-n-mine&platform=windows) | [macOS](https://dinamika-games.github.io/download.html?game=jump-n-mine&platform=macos) | [Linux](https://dinamika-games.github.io/download.html?game=jump-n-mine&platform=linux)
- **Splash 'n' Splat** — [Windows](https://dinamika-games.github.io/download.html?game=splash-n-splat&platform=windows) | [macOS](https://dinamika-games.github.io/download.html?game=splash-n-splat&platform=macos) | [Linux](https://dinamika-games.github.io/download.html?game=splash-n-splat&platform=linux)
- **Steppe Rescue** — [Windows](https://dinamika-games.github.io/download.html?game=steppe-rescue&platform=windows) | [macOS](https://dinamika-games.github.io/download.html?game=steppe-rescue&platform=macos) | [Linux](https://dinamika-games.github.io/download.html?game=steppe-rescue&platform=linux)

# Manifesto of Dinamika Games

A shadow hangs over the children's room: the shadow of the glowing screen.
All the powers of the attention economy have joined forces to keep it there: the app store and the ad network, the feed and the leaderboard, the loot box and the push notification.

Two things follow from this.
First, the way we play is no longer a private matter; it has become a question of what kind of people we are raising.
Second, it is time for those who make games to say openly what they stand for, and to set this manifesto against the silence of the industry.

## I. Players and Consumers

The history of all play until now has been the history of bodies in motion.
Children chased each other through the streets, built forts, danced in circles and made up rules that lasted a single afternoon.
Play was shared, loud and outdoors, and no one had to be destroyed for it to end.

The modern game industry has put an end to all of this.
It has pulled the player out of the yard and sat them down on the sofa.
It has turned the companion into an opponent and the opponent into a target.
It has left no bond between player and player other than the naked scoreboard.
It has drowned the joy of shared play in the icy water of winner-takes-all.

Short-lived media in the format of a goldfish has done the same to attention.
What once held a child for an afternoon now holds them for fifteen seconds, and then the next fifteen, and the next.

We do not claim that games kill people.
Games do not kill people; people with guns kill people.
But the view of the world that a game carries does not stay inside the game.
Children take it on and carry it long after the screen is dark, without knowing they carry it.
Compete instead of cooperate.
The winner takes everything; the others go home with nothing.
Sit still, do not move, consume.

## II. Dinamika and the Players

What do we want?
We want games for a world that is collaborative, active and free of violence.

We put:

- collaboration in place of competition;
- shared success in place of winner-takes-all;
- moving bodies in place of still bodies;
- playing together in one room in place of consuming alone on a sofa;
- challenge in place of violence;
- sustained attention in place of short-lived stimulation.

In our games, the following will apply:

1. Players finish a game closer to each other than when they started.
2. A game is won together or not at all; when one player fails, the group helps.
3. Players use their bodies: they stand up, walk, jump, point, dance and reach for each other.
4. Tension comes from puzzles, timing, rhythm and the unknown, never from hurting someone.
5. A game shows a world, and it must be a world we want our children to live in.
6. Players talk to each other face to face; the screen serves the group and does not replace it.
7. Children, parents and grandparents play in the same game, each with a real part to play.
8. A session has a clear end, and stopping is always easy.
9. No endless feeds, no loot boxes, no tricks to pull players back.
10. Simple rules leave room to invent; players may bend the game and make it their own.

## III. Conclusion

Dinamika does not hide its views and aims.
We openly declare that our ends can be reached only by changing the games our children grow up with.
Let the makers of violent worlds tremble before a generation that has learned to play together.
Players have nothing to lose but their sofas.
They have a world to share.

**Players of the world, unite!**
