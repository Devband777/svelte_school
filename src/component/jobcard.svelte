<script>
    let coin = './lib/images/Coin.png';
</script>
<div class="job_post">
    <div class="job_content">
        <div class="support_text">
            <p class="bodyM">MYP Design Teacher</p>
            <span class="body2R">We are looking for a MYP Design teacher to join our team.</span>
            <div class="view_job_btn">
                <span class="btn">View Job</span>
            </div>
        </div>
        <div class="details">
            <div class="location">
                <span class="body2M">Vijayawada, India</span>
            </div>
            <div class="worktype">
                <span class="body2M">Full Time</span>
            </div>
            <div class="salary">
                <span class="body2M"><img src={coin} alt="">500-3000$</span>
            </div>
        </div>
    </div>
</div>
<style lang="scss">
    .job_post {
        align-items: center;
        padding: 48px;
        gap: 24px;
        width: 130%;
        height: 30%;
        background: #FFFFFF;
        box-shadow: 0px 4px 80px rgba(68, 40, 14, 0.1);
        border-radius: 24px;
   
        .job_content {
            padding: 0px;
            gap: 32px;
            width: 100%;
            height: 0%;

            .support_text {
                position: relative;
                margin-bottom: 10%;

                .view_job_btn {
                    position: absolute;
                    top: 0;
                    right: 0;
                }
            }
            .details {
                position: relative;

                .location {
                    position: absolute;
                    left: 0;
                }
                .worktype {
                    position: absolute;
                    left: 40%;
                }
                .salary {
                    position: absolute;
                    left: 70%;
                }
            }
        }
    }
</style>