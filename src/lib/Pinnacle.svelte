<script>
  import Icons from './Icons.svelte'

  export let name
  export let title
  export let phone

  // images must load remotely from an absolute URL to be reliable
  export const imagesBaseUrl =
    'https://pb.haume.nz/api/files/amu003xvt8ezymb/5bzgq2zi74wllgj/'
  export const fonts =
    'font-size: medium; font-family: Helvetica, Arial, sans-serif;'
  const logoUrl = imagesBaseUrl + '/pinnacle_orig_z5ehslwzwt.jpg'
</script>

<!-- Horrendous HTML and CSS as recommended for email signatures. -->
<table style={fonts} cellspacing="0" cellpadding="0">
  <tbody>
    <tr>
      <td>
        <table style={fonts} cellspacing="0" cellpadding="0">
          <tbody>
            <tr>
              <td style="vertical-align: top">
                <img
                  src={logoUrl}
                  role="presentation"
                  style="display: block; max-width: 170px"
                  width="170"
                  alt="" />
              </td>
              <!-- <td style="padding-left: 29px; border-right: 1px solid #8EA5C7;">
                <div />
              </td> -->
              <td style="padding-left: 29px; vertical-align: middle">
                <h2
                  color="#0C0732"
                  style="
                    margin: 0px;
                    font-size: 16pt;
                    color: #0C0732;
                    font-weight: 600;
                    line-height: 30px;
                  ">
                  {name.toUpperCase()}
                </h2>
                <p
                  color="#0C0732"
                  style="
                    margin: 0px;
                    color: #0C0732;
                    font-size: 14pt;
                    font-weight: 600;
                    line-height: 25px;
                  ">
                  {title}
                </p>

                <p
                  color="#0C0732"
                  style="
                    margin: 0px;
                    color: #0C0732;
                    font-size: 14pt;
                    font-weight: 600;
                    line-height: 25px;
                  ">
                  Pinnacle Post
                </p>

                <p
                  color="#0C0732"
                  style="
                    margin: 0px;
                    color: #0C0732;
                    font-size: 14pt;
                    font-weight: 600;
                    line-height: 25px;
                  ">
                  {phone}
                </p>
                <p
                  style="
                    margin: 0px;
                    font-size: 13pt;
                    line-height: 25px;
                ">
                  <a
                    style="text-decoration: none; font-weight: 400; color: #467886;"
                    href="https://www.pinnaclepost.co.nz"
                    >www.pinnaclepost.co.nz</a>
                </p>
                <p>
                  <a
                    href="https://www.linkedin.com/company/pinnacle-post/"
                    style="
                    display: inline-block;
                    padding: 0px;
                  ">
                    <img
                      alt=""
                      src={`${imagesBaseUrl}/cn_p_24092025_160248_04zhf8k340.png`}
                      style="
                      max-width: 34px;
                      display: block;
                    "
                      height="34" /></a>
                  <a
                    href="https://www.instagram.com/pinnaclepost_nz/"
                    style="
                      display: inline-block;
                      padding: 0px;
                    ">
                    <img
                      alt=""
                      src={`${imagesBaseUrl}/cn_p_24092025_160051_uvub5igo9o.png`}
                      style="
                        max-width: 34px;
                        display: block;
                      "
                      height="34" /></a>
                </p>
              </td>
            </tr>
          </tbody>
        </table>
      </td>
    </tr>
    <!-- <tr
      ><td colspan="2"
        ><p
          style="                    padding-top: 10px;
        font-size: 10pt; color: #adadad;">
          This e-mail is for the sole use of the intended recipient(s). It
          contains information that may be confidential. If you believe that it
          has been sent to you in error, please notify the sender immediately by
          reply e-mail and destroy all copies of this message. Any disclosure,
          copying, distribution, or use of this information by anyone other than
          the intended recipient is prohibited.
        </p></td>
    </tr> -->
  </tbody>
</table>

<style>
  /* Must use inline styles with email. */
</style>
