<template>
  <q-page class="flex flex-center fullscreen">
    <video ref="video" class="video-js fit" playsinline />
  </q-page>
</template>

<script>
import { defineComponent, ref } from "vue";
import { useQuasar } from "quasar";
import videojs from "video.js";
import "video.js/dist/video-js.css";

export default defineComponent({
  name: "IndexPage",

  setup() {
    const $q = useQuasar();
    const loop = ref(false);
    const player = ref(null);
    const video = ref(null);
    const videoSrc = ref("~assets/video-0.mp4");

    return {
      q: $q,
      loop,
      player,
      video,
      videoSrc,
      videoOptions: {
        controls: false,
      },
    };
  },
  created() {
    // Key press event
    window.addEventListener("keydown", (e) => {

      switch (e.key) {
        /**********************
         * Spacebar
         **********************/
        case " ":
          // if player is paused, then play. If playing, then pause.
          this.player.paused() ? this.player.play() : this.player.pause();
          break;

        /**********************
         * Enter
         **********************/
        case "Enter":
          this.player.poster("/src/assets/video-intro.jpg");
          // then the video source
          this.player.src({
            src: "/src/assets/video-intro.mp4",
            type: "video/mp4",
          });
          // is this player looping?
          this.player.loop(true);
          // launch app in fullscreen
          this.q.fullscreen
            .request()
            .then(() => {
              // now play the video
              this.player.play();
            })
            .catch((err) => {
              console.log(err);
            });
          break;

        /**********************
         * Escape
         **********************/
        case "Escape":
          // pause video
          this.player.pause();
          // exit fullscreen
          this.q.fullscreen
            .exit()
            .then(() => {})
            .catch((err) => {
              console.log(err);
            });
          break;

        /**********************
         * a
         **********************/
        case "a":
          // set the poster for this video first
          this.player.poster("/src/assets/video-a.jpg");
          // then the video source
          this.player.src({
            src: "/src/assets/video-a.mp4",
            type: "video/mp4",
          });
          // is this player looping?
          this.player.loop(false);
          // now play the video
          this.player.play();
          break;

        /**********************
         * b
         **********************/
        case "b":
          // set the poster for this video first
          this.player.poster("/src/assets/video-b.jpg");
          // then the video source
          this.player.src({
            src: "/src/assets/video-b.mp4",
            type: "video/mp4",
          });
          // is this player looping?
          this.player.loop(false);
          // now play the video
          this.player.play();
          break;

        /**********************
         * c
         **********************/
        case "c":
          // set the poster for this video first
          this.player.poster("/src/assets/video-c.jpg");
          // then the video source
          this.player.src({
            src: "/src/assets/video-c.mp4",
            type: "video/mp4",
          });
          // is this player looping?
          this.player.loop(false);
          // now play the video
          this.player.play();
          break;

        /**********************
         * d
         **********************/
        case "d":
          // set the poster for this video first
          this.player.poster("/src/assets/video-d.jpg");
          // then the video source
          this.player.src({
            src: "/src/assets/video-d.mp4",
            type: "video/mp4",
          });
          // is this player looping?
          this.player.loop(false);
          // now play the video
          this.player.play();
          break;

        /**********************
         * e
         **********************/
        case "e":
          // set the poster for this video first
          this.player.poster("/src/assets/video-e.jpg");
          // then the video source
          this.player.src({
            src: "/src/assets/video-e.mp4",
            type: "video/mp4",
          });
          // is this player looping?
          this.player.loop(false);
          // now play the video
          this.player.play();
          break;

        /**********************
         * f
         **********************/
        case "f":
          // set the poster for this video first
          this.player.poster("/src/assets/video-f.jpg");
          // then the video source
          this.player.src({
            src: "/src/assets/video-f.mp4",
            type: "video/mp4",
          });
          // is this player looping?
          this.player.loop(false);
          // now play the video
          this.player.play();
          break;

        /**********************
         * g
         **********************/
        case "g":
          // set the poster for this video first
          this.player.poster("/src/assets/video-g.jpg");
          // then the video source
          this.player.src({
            src: "/src/assets/video-g.mp4",
            type: "video/mp4",
          });
          // is this player looping?
          this.player.loop(false);
          // now play the video
          this.player.play();
          break;

        /**********************
         * h
         **********************/
        case "h":
          // set the poster for this video first
          this.player.poster("/src/assets/video-h.jpg");
          // then the video source
          this.player.src({
            src: "/src/assets/video-h.mp4",
            type: "video/mp4",
          });
          // is this player looping?
          this.player.loop(false);
          // now play the video
          this.player.play();
          break;

        /**********************
         * i
         **********************/
        case "i":
          // set the poster for this video first
          this.player.poster("/src/assets/video-i.jpg");
          // then the video source
          this.player.src({
            src: "/src/assets/video-i.mp4",
            type: "video/mp4",
          });
          // is this player looping?
          this.player.loop(false);
          // now play the video
          this.player.play();
          break;

        /**********************
         * h
         **********************/
        case "j":
          // set the poster for this video first
          this.player.poster("/src/assets/video-j.jpg");
          // then the video source
          this.player.src({
            src: "/src/assets/video-j.mp4",
            type: "video/mp4",
          });
          // is this player looping?
          this.player.loop(false);
          // now play the video
          this.player.play();
          break;

        /**********************
         * h
         **********************/
        case "k":
          // set the poster for this video first
          this.player.poster("/src/assets/video-k.jpg");
          // then the video source
          this.player.src({
            src: "/src/assets/video-k.mp4",
            type: "video/mp4",
          });
          // is this player looping?
          this.player.loop(false);
          // now play the video
          this.player.play();
          break;

        /**********************
         * l
         **********************/
        case "l":
          // set the poster for this video first
          this.player.poster("/src/assets/video-l.jpg");
          // then the video source
          this.player.src({
            src: "/src/assets/video-l.mp4",
            type: "video/mp4",
          });
          // is this player looping?
          this.player.loop(false);
          // now play the video
          this.player.play();
          break;

        /**********************
         * m
         **********************/
        case "m":
          // set the poster for this video first
          this.player.poster("/src/assets/video-m.jpg");
          // then the video source
          this.player.src({
            src: "/src/assets/video-m.mp4",
            type: "video/mp4",
          });
          // is this player looping?
          this.player.loop(false);
          // now play the video
          this.player.play();
          break;

        /**********************
         * n
         **********************/
        case "n":
          // set the poster for this video first
          this.player.poster("/src/assets/video-n.jpg");
          // then the video source
          this.player.src({
            src: "/src/assets/video-n.mp4",
            type: "video/mp4",
          });
          // is this player looping?
          this.player.loop(false);
          // now play the video
          this.player.play();
          break;

        /**********************
         * o
         **********************/
        case "o":
          // set the poster for this video first
          this.player.poster("/src/assets/video-o.jpg");
          // then the video source
          this.player.src({
            src: "/src/assets/video-o.mp4",
            type: "video/mp4",
          });
          // is this player looping?
          this.player.loop(false);
          // now play the video
          this.player.play();
          break;

        /**********************
         * o
         **********************/
        case "p":
          // set the poster for this video first
          this.player.poster("/src/assets/video-p.jpg");
          // then the video source
          this.player.src({
            src: "/src/assets/video-p.mp4",
            type: "video/mp4",
          });
          // is this player looping?
          this.player.loop(false);
          // now play the video
          this.player.play();
          break;

        /**********************
         * o
         **********************/
        case "q":
          // set the poster for this video first
          this.player.poster("/src/assets/video-q.jpg");
          // then the video source
          this.player.src({
            src: "/src/assets/video-q.mp4",
            type: "video/mp4",
          });
          // is this player looping?
          this.player.loop(false);
          // now play the video
          this.player.play();
          break;

        /**********************
         * r
         **********************/
        case "r":
          // set the poster for this video first
          this.player.poster("/src/assets/video-r.jpg");
          // then the video source
          this.player.src({
            src: "/src/assets/video-r.mp4",
            type: "video/mp4",
          });
          // is this player looping?
          this.player.loop(false);
          // now play the video
          this.player.play();
          break;

        default:
      }
    });
  },
  mounted() {
    this.player = videojs(this.video, this.videoOptions, () => {
      this.player.log("onPlayerReady", this);
    });
  },
  beforeUnmount() {
    if (this.player) {
      this.player.dispose();
      window.removeEventListener("keydown", {});
    }
  },
});
</script>
