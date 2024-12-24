<template>
    <div class="dropdown">
        <input type="checkbox" id="dropdown" name="dropdown">
        <label for="dropdown" class="dropdown-btn">

            <span class="dropdown-txt">
                <span class="dropdown-txt-fst">Офис на </span>
                Малиновского
            </span>
            <svg width="8" height="8" viewBox="0 0 8 8" xmlns="http://www.w3.org/2000/svg">
                <path d="M0.5 3.5V2.5H1.5V3.5H0.5Z" />
                <path d="M2.5 4.5H1.5V3.5H2.5V4.5Z" />
                <path d="M3.5 5.5H2.5V4.5H3.5V5.5Z" />
                <path d="M4.5 5.5V6.5H3.5V5.5H4.5Z" />
                <path d="M5.5 4.5V5.5H4.5V4.5H5.5Z" />
                <path d="M6.5 3.5H5.5V4.5H6.5V3.5Z" />
                <path d="M6.5 3.5H7.5V2.5H6.5V3.5Z" />
            </svg>
        </label>
        <ul class="dropdown-list">
            <li>new</li>
        </ul>
    </div>
</template>



<script setup>

</script>


<style scoped lang="scss">
@media (min-width: 1920px) {
    .dropdown {
        margin: 0 0 18px 0;

        & input {
            display: none;
        }

        &>input {
            &:checked~ {
                .header-mini--info-wrap--micro-dropdown-list {
                    display: block;
                }
            }
        }

        &-txt {
            &-fst {
                display: inline-block;
            }
        }

        &-btn {
            display: flex;
            padding: 0;
            border: none;
            color: #222222;
            text-align: left;
            background: none;

            & svg {
                margin: 8px 0;
                margin-left: 8px;
                fill: #222222;
            }
        }

        &-list {
            display: none;
            //padding: 0;
            //list-style: none;
        }


    }
}
@media (max-width: 1920px) {
    .dropdown {
        margin: 0 0 18px 0;

        & input {
            display: none;
        }

        &>input {
            &:checked~ {
                .header-mini--info-wrap--micro-dropdown-list {
                    display: block;
                }
            }
        }

        &-txt {
            &-fst {
                display: inline-block;
            }
        }

        &-btn {
            display: flex;
            padding: 0;
            border: none;
            color: #222222;
            text-align: left;
            background: none;

            & svg {
                margin: 8px 0;
                margin-left: 8px;
                fill: #222222;
            }
        }

        &-list {
            display: none;
            //padding: 0;
            //list-style: none;
        }


    }
}

@media (max-width: 1280px) {
    .dropdown {
        &-txt {
            &-fst {
                display: none;
            }
        }
    }
}
</style>