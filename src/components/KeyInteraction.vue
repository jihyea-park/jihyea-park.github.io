<template>
    <div class="backdrop" v-if="theme === 'Q'">
        <div class="modal" :class="{ q: theme === 'Q' }">
            <video src="http://127.0.0.1:8887/video/clip_a1_1.mp4" autoplay></video>
        </div>
    </div>
    <div class="backdrop" v-if="theme === 'W'">
        <div class="modal" :class="{ w: theme === 'W' }">
            <video src="http://127.0.0.1:8887/video/clip_a3.mp4" autoplay></video>
        </div>
    </div>
    <div class="backdrop" v-if="theme === 'E'">
        <div class="modal" :class="{ e: theme === 'E' }">
            <video src="http://127.0.0.1:8887/video/clip_a3_2.mp4" autoplay></video>
        </div>
    </div>
    <div class="backdrop" v-if="theme === 'A'">
        <div class="modal" :class="{ a: theme === 'A' }">
            <video src="http://127.0.0.1:8887/video/clip_a3_5.mp4" autoplay></video>
        </div>
    </div>
    <div class="backdrop" v-if="theme === 'S'">
        <div class="modal" :class="{ s: theme === 'S' }">
            <video src="http://127.0.0.1:8887/video/clip_b1_4.mp4" autoplay></video>
        </div>
    </div>
    <div class="backdrop" v-if="theme === 'D'">
        <div class="modal" :class="{ d: theme === 'D' }">
            <video src="http://127.0.0.1:8887/video/clip_b2_3.mp4" autoplay></video>
        </div>
    </div>
    <div class="backdrop" v-if="theme === 'Y'">
        <div class="modal" :class="{ y: theme === 'Y' }">
            <video src="http://127.0.0.1:8887/video/clip_b3_2_1.mp4" autoplay></video>
        </div>
    </div>
    <div class="backdrop" v-if="theme === 'X'">
        <div class="modal" :class="{ x: theme === 'X' }">
            <video src="http://127.0.0.1:8887/video/clip_b3_5_1.mp4" autoplay></video>
        </div>
    </div>
    <div class="backdrop" v-if="theme === 'C'">
        <div class="modal" :class="{ c: theme === 'C' }">
            <video src="http://127.0.0.1:8887/video/clip_b1_4_1.mp4" autoplay></video>
        </div>
    </div>
    <div class="backdrop" v-if="theme === 'V'">
        <div class="modal" :class="{ v: theme === 'V' }">
            <video src="http://127.0.0.1:8887/video/clip_b2_3_1.mp4" autoplay></video>
        </div>
    </div>
    <div class="backdrop" v-if="theme === 'R'">
        <div class="modal" :class="{ r: theme === 'R' }">
            <video src="http://127.0.0.1:8887/video/clip_a1_0.mp4" autoplay></video>
        </div>
    </div>
    <div class="backdrop" v-if="theme === 'T'">
        <div class="modal" :class="{ t: theme === 'T' }">
            <video src="http://127.0.0.1:8887/video/clip_a2_0.mp4" autoplay></video>
        </div>
    </div>
    <div class="backdrop" v-if="theme === 'Z'">
        <div class="modal" :class="{ z: theme === 'Z' }">
            <video src="http://127.0.0.1:8887/video/clip_a3_0.mp4" autoplay></video>
        </div>
    </div>
    <div class="backdrop" v-if="theme === 'U'">
        <div class="modal" :class="{ u: theme === 'U' }">
            <video src="http://127.0.0.1:8887/video/clip_a4_0.mp4" autoplay></video>
        </div>
    </div>
    <div class="backdrop" v-if="theme === 'I'">
        <div class="modal" :class="{ i: theme === 'I' }">
            <video src="http://127.0.0.1:8887/video/clip_a6.mp4" autoplay></video>
        </div>
    </div>
    <div class="backdrop" v-if="theme === 'O'">
        <div class="modal" :class="{ o: theme === 'O' }">
            <video src="http://127.0.0.1:8887/video/clip_a8.mp4" autoplay></video>
        </div>
    </div>
    <div class="backdrop" v-if="theme === 'P'">
        <div class="modal" :class="{ p: theme === 'P' }">
            <video src="http://127.0.0.1:8887/video/clip_a9.mp4" autoplay></video>
        </div>
    </div>
    <div class="backdrop" v-if="theme === 'Ü'">
        <div class="modal" :class="{ ue: theme === 'Ü' }">
            <video src="http://127.0.0.1:8887/video/clip_1n.mp4" autoplay></video>
        </div>
    </div>
    <div class="backdrop" v-if="theme === 'Ö'">
        <div class="modal" :class="{ oe: theme === 'O' }">
            <video src="http://127.0.0.1:8887/video/clip_1n_1.mp4" autoplay></video>
        </div>
    </div>
    <div class="backdrop" v-if="theme === 'Ä'">
        <div class="modal" :class="{ ae: theme === 'Ä' }">
            <video src="http://127.0.0.1:8887/video/clip_3n.mp4" autoplay></video>
        </div>
    </div>
    <div class="backdrop" v-if="theme === 'F'">
        <div class="modal" :class="{ f: theme === 'F' }">
            <video src="http://127.0.0.1:8887/video/clip_b1.mp4" autoplay></video>
        </div>
    </div>
    <div class="backdrop" v-if="theme === 'G'">
        <div class="modal" :class="{ g: theme === 'G' }">
            <video src="http://127.0.0.1:8887/video/clip_b2.mp4" autoplay></video>
        </div>
    </div>
    <div class="backdrop" v-if="theme === 'H'">
        <div class="modal" :class="{ h: theme === 'H' }">
            <video src="http://127.0.0.1:8887/video/clip_b3.mp4" autoplay></video>
        </div>
    </div>
    <div class="backdrop"  v-if="theme === 'J'">
        <div class="modal" :class="{ j: theme === 'J' }">
            <video src="http://127.0.0.1:8887/video/clip_b5.mp4" autoplay></video>
        </div>
    </div>
    <div class="backdrop"  v-if="theme === 'K'">
        <div class="modal" :class="{ k: theme === 'K' }">
            <video src="http://127.0.0.1:8887/video/clip_b6_1.mp4" autoplay></video>
        </div>
    </div>
    <div class="backdrop"  v-if="theme === 'L'">
        <div class="modal" :class="{ l: theme === 'L' }">
            <video src="http://127.0.0.1:8887/video/clip_b7.mp4" autoplay></video>
        </div>
    </div>
    <div class="backdrop"  v-if="theme === 'B'">
        <div class="modal" :class="{ b: theme === 'B' }">
            <video src="http://127.0.0.1:8887/video/clip_b8.mp4" autoplay></video>
        </div>
    </div>
    <div class="backdrop"  v-if="theme === 'N'">
        <div class="modal" :class="{ n: theme === 'N' }">
            <video src="http://127.0.0.1:8887/video/clip_b9.mp4" autoplay></video>
        </div>
    </div>
    <div class="backdrop"  v-if="theme === 'M'">
        <div class="modal" :class="{ m: theme === 'M' }">
            <video src="http://127.0.0.1:8887/video/clip_b10.mp4" autoplay></video>
        </div>
    </div>
    <div class="backdrop"  v-if="theme === ','">
        <div class="modal" :class="{ comma: theme === ',' }">
            <video src="http://127.0.0.1:8887/video/clip_b11_1.mp4" autoplay></video>
        </div>
    </div>
    <div class="backdrop"  v-if="theme === '.'">
        <div class="modal" :class="{ dot: theme === '.' }">
            <video src="http://127.0.0.1:8887/video/clip_b11_2.mp4" autoplay></video>
        </div>
    </div>
</template>

<script>
export default {
    props: ['theme'],
}
</script>

<style>

    body {
        pointer-events: none;
    }

    .backdrop {
        top: 0;
        position: fixed;
        /* background: rgba(0, 0, 0, 0.6); */
        width: 100%;
        height: 100%;
    }

    img {
        width: 100%;
        height: 100%;
    }

    video {
        width: 80%;
        height: 80%;
    }

    .backdrop .modal.q {
        background: rgba(0,0,0,0.3);
        width: 100%;
        height: 100%;
    }

    .backdrop .modal.w {
        background: rgba(0,0,0,0.3);
        width: 100%;
        height: 100%;
    }

    .backdrop .modal.e {
        background: rgba(0,0,0,0.3);
        width: 100%;
        height: 100%;
    }

    .backdrop .modal.a {
        background: rgba(0,0,0,0.3);
        width: 100%;
        height: 100%;
    }

    .backdrop .modal.s {
        background: rgba(0,0,0,0.3);
        width: 100%;
        height: 100%;
    }

    .backdrop .modal.d {
        background: rgba(0,0,0,0.3);
        width: 100%;
        height: 100%;
    }

    .backdrop .modal.y {
        background: rgba(0,0,0,0.3);
        width: 100%;
        height: 100%;
    }

    .backdrop .modal.x {
        background: rgba(0,0,0,0.3);
        width: 100%;
        height: 100%;
    }

    .backdrop .modal.c {
        background: rgba(0,0,0,0.3);
        width: 100%;
        height: 100%;
    }

    .backdrop .modal.v {
        background: rgba(0,0,0,0.3);
        width: 100%;
        height: 100%;
    }

</style>